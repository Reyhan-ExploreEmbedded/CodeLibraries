################################################################################
# Automatically-generated file. Do not edit!
################################################################################

SHELL := cmd.exe
RM := rm -rf

USER_OBJS :=

LIBS := 
PROJ := 

O_SRCS := 
C_SRCS := 
S_SRCS := 
S_UPPER_SRCS := 
OBJ_SRCS := 
ASM_SRCS := 
PREPROCESSING_SRCS := 
OBJS := 
OBJS_AS_ARGS := 
C_DEPS := 
C_DEPS_AS_ARGS := 
EXECUTABLES := 
OUTPUT_FILE_PATH :=
OUTPUT_FILE_PATH_AS_ARGS :=
AVR_APP_PATH :=$$$AVR_APP_PATH$$$
QUOTE := "
ADDITIONAL_DEPENDENCIES:=
OUTPUT_FILE_DEP:=

# Every subdirectory with source files must be described here
SUBDIRS := 


# Add inputs and outputs from these tool invocations to the build variables 
C_SRCS +=  \
../delay.c \
../eeprom.c \
../Eeprom_CharRdWr_Uart.c \
../uart.c


PREPROCESSING_SRCS += 


ASM_SRCS += 


OBJS +=  \
delay.o \
eeprom.o \
Eeprom_CharRdWr_Uart.o \
uart.o


OBJS_AS_ARGS +=  \
delay.o \
eeprom.o \
Eeprom_CharRdWr_Uart.o \
uart.o


C_DEPS +=  \
delay.d \
eeprom.d \
Eeprom_CharRdWr_Uart.d \
uart.d


C_DEPS_AS_ARGS +=  \
delay.d \
eeprom.d \
Eeprom_CharRdWr_Uart.d \
uart.d


OUTPUT_FILE_PATH +=Eeprom_CharRdWr_Uart.elf

OUTPUT_FILE_PATH_AS_ARGS +=Eeprom_CharRdWr_Uart.elf

ADDITIONAL_DEPENDENCIES:=

OUTPUT_FILE_DEP:= ./makedep.mk

# AVR32/GNU C Compiler









./%.o: .././%.c
	@echo Building file: $<
	@echo Invoking: AVR/GNU C Compiler : (WinAVR 20100110) 4.3.3
	$(QUOTE)C:\WinAVR-20100110\bin\avr-gcc.exe$(QUOTE) -funsigned-char -funsigned-bitfields -DF_CPU=16000000  -Os -fpack-struct -fshort-enums -g2 -Wall -c -std=gnu99 -MD -MP -MF "$(@:%.o=%.d)" -MT"$(@:%.o=%.d)" -MT"$(@:%.o=%.o)"  -mmcu=atmega16   -o"$@" "$<" 
	@echo Finished building: $<



# AVR32/GNU Preprocessing Assembler



# AVR32/GNU Assembler




ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: $(OUTPUT_FILE_PATH) $(ADDITIONAL_DEPENDENCIES)

$(OUTPUT_FILE_PATH): $(OBJS) $(USER_OBJS) $(OUTPUT_FILE_DEP)
	@echo Building target: $@
	@echo Invoking: AVR/GNU Linker : (WinAVR 20100110) 4.3.3
	$(QUOTE)C:\WinAVR-20100110\bin\avr-gcc.exe$(QUOTE) -o$(OUTPUT_FILE_PATH_AS_ARGS) $(OBJS_AS_ARGS) $(USER_OBJS) $(LIBS) -Wl,-Map="Eeprom_CharRdWr_Uart.map" -Wl,--start-group -Wl,-lm  -Wl,--end-group  -mmcu=atmega16  
	@echo Finished building target: $@
	"C:\WinAVR-20100110\bin\avr-objcopy.exe" -O ihex -R .eeprom -R .fuse -R .lock -R .signature  "Eeprom_CharRdWr_Uart.elf" "Eeprom_CharRdWr_Uart.hex"
	"C:\WinAVR-20100110\bin\avr-objcopy.exe" -j .eeprom  --set-section-flags=.eeprom=alloc,load --change-section-lma .eeprom=0  --no-change-warnings -O ihex "Eeprom_CharRdWr_Uart.elf" "Eeprom_CharRdWr_Uart.eep" || exit 0
	"C:\WinAVR-20100110\bin\avr-objdump.exe" -h -S "Eeprom_CharRdWr_Uart.elf" > "Eeprom_CharRdWr_Uart.lss"
	"C:\WinAVR-20100110\bin\avr-size.exe" "Eeprom_CharRdWr_Uart.elf"
	





# Other Targets
clean:
	-$(RM) $(OBJS_AS_ARGS)$(C_DEPS_AS_ARGS) $(EXECUTABLES) 
	rm -rf "Eeprom_CharRdWr_Uart.elf" "Eeprom_CharRdWr_Uart.a" "Eeprom_CharRdWr_Uart.hex" "Eeprom_CharRdWr_Uart.lss" "Eeprom_CharRdWr_Uart.eep" "Eeprom_CharRdWr_Uart.map"
	