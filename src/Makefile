C=gcc
CFLAGS=-I.
DEPS = ICM20948.h ICM20948_registers.h msb_imu.h
OBJ = msb_imu.o msb_imu_i2c.o 

%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

msb_imu: $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS)


