# SPDX-License-Identifier: Apache-2.0

zephyr_sources_ifdef(CONFIG_CAN              can_common.c)
zephyr_sources_ifdef(CONFIG_CAN_LOOPBACK     can_loopback.c)
zephyr_sources_ifdef(CONFIG_CAN_MCP2515      can_mcp2515.c)
zephyr_sources_ifdef(CONFIG_CAN_STM32        can_stm32.c)
zephyr_sources_ifdef(CONFIG_CAN_MCUX_FLEXCAN can_mcux_flexcan.c)

zephyr_sources_ifdef(CONFIG_USERSPACE        can_handlers.c)
zephyr_sources_ifdef(CONFIG_CAN_SHELL        can_shell.c)
