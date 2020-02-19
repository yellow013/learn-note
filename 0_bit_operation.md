

清除Int高位: i & 0x0000ffff

清除Int低位: i & 0xffff0000

获得最接近的2的幂次方:

int minPow2(int i) {
		int n = i - 1;
		n |= n >>> 1;
		n |= n >>> 2;
		n |= n >>> 4;
		n |= n >>> 8;
		n |= n >>> 16;
    int max = 1 << 30;
		return (n < 0) ? 1 : (n >= max) ? max : n + 1;
}
