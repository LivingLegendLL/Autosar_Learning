- Arbitrate mode requests from SWC's or other BSW modules
- Mode arbitration - based on request received initiates mode requests or provides mode indications. All done via Request/Mode port interface. Based on user request
- Mode Control - mode switches by execution of action lists. Cyclic checks. Input sequence is configured and when it is satisfied it will execute (ex.: wakeup conditions)
- Works along side with [[BswM]] and [[EcuM]]
- *BSWMModeRequestPort* (ASWC requests Full Com) / *BSWMModeConditions* (Init state of [[ComM]] and ASWC request) / *BSWMLogicalExpressions* (ASWC request && init state of [[CAN SM]] / [[ComM]]) / *BSWMActions* (Switch to Full Com) / *BSWMActionlists* (multiple actions) / *BSWMRules* (container that includes all above. Condition can be arbitration or control)
- ![Pasted image 20230615112410](https://github.com/LivingLegendLL/Autosar_Learning/assets/125698571/d54c6709-83d0-4f24-b514-cb9f29a6d860)