##eco-flowchart на примере Top Trading Cycle (TTC)

- [Top Trading Cycle](https://en.wikipedia.org/wiki/Top_trading_cycle) - Wikipedia

***

```json
{
    "s_000_v__init_state": { "state_info":{"name":"Init state"},
                            "v_00":"s_000_v__init_state",             "00":   "Init",
                            "v_10":"s_010_v__promt_need_instruction", "10":   "Ask: Ready or Need to read Instruction"
                        },
    "s_010_v__promt_need_instruction": { "state_info":{"name":"Ask: Ready or Need to read Instruction"},
                            "v_10":"s_030_v__instruction",    "10":   "Let's show instruction",
                            "v_20":"s_040_v__agreement",      "20":   "Show Agreement"
                        },
    "s_030_v__instruction": { "state_info":{"name":"Show instruction"},
                            "v_10":"s_040_v__agreement",      "10":   "Show agreement"
                        },
    "s_040_v__agreement": { "state_info":{"name":"Show agreement. Ask: Agree or not"},
                            "v_10":"s_050__start_questionnaire",        "10":   "if agree",
                            "v_20":"s_800_v__quit_questionnaire",  "20":   "if not agree"
                        },
    "s_050__start_questionnaire": { "state_info":{"name":"Start questions"},
                            "v_10":"s_060_v__questions",  "10":   "Continue"
                        },
    "s_060_v__questions": { "state_info":{"name":"Ask questions"},
                            "v_10":"s_060_v__questions",  "10":   "Next question",
                            "v_20":"s_070_v__show_result",  "20":   "Show result"
                        },
    "s_070_v__show_result": { "state_info":{"name":"Show result"},
                            "v_10":"s_050__start_questionnaire",  "10":   "Try again"
                        },
    "s_800_v__quit_questionnaire": { "state_info":{"name":"Quit questionnaire"}

                        }
}
```
