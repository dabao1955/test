# 定义 scx.o 由哪些 .o 组成
scx-objs := scx_shadow_tick.o \
            cpufreq_scx_main.o \
            hmbird_gki/scx_util_track.o \
            hmbird_gki/scx_sched_gki.o \
            hmbird_gki/scx_main.o

# 根据配置决定是否编译 scx.o 到 built-in.a
obj-$(CONFIG_HMBIRD_SCHED_GKI) += scx.o

# 如果 main.o 是独立的（不依赖 scx-objs），也可以单独加
# obj-$(CONFIG_HMBIRD_SCHED_GKI) += main.o
