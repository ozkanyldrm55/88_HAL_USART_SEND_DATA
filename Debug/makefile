################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
88_HAL_USART_SEND_DATA.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
88_HAL_USART_SEND_DATA.list \

OBJCOPY_BIN += \
88_HAL_USART_SEND_DATA.bin \


# All Target
all: 88_HAL_USART_SEND_DATA.elf secondary-outputs

# Tool invocations
88_HAL_USART_SEND_DATA.elf: $(OBJS) $(USER_OBJS) C:\Users\AR-GE\ PC\Desktop\arm\88_HAL_USART_SEND_DATA\STM32F407VGTX_FLASH.ld
	arm-none-eabi-gcc -o "88_HAL_USART_SEND_DATA.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\AR-GE PC\Desktop\arm\88_HAL_USART_SEND_DATA\STM32F407VGTX_FLASH.ld" --specs=nosys.specs -Wl,-Map="88_HAL_USART_SEND_DATA.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

88_HAL_USART_SEND_DATA.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "88_HAL_USART_SEND_DATA.list"
	@echo 'Finished building: $@'
	@echo ' '

88_HAL_USART_SEND_DATA.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "88_HAL_USART_SEND_DATA.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
