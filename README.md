﻿﻿﻿﻿﻿﻿# Hotel_System_master### hotel员工管理系统mysql```/* Navicat Premium Data Transfer Source Server         : localhost Source Server Type    : MySQL Source Server Version : 100126 Source Host           : localhost:3306 Source Schema         : hotel Target Server Type    : MySQL Target Server Version : 100126 File Encoding         : 65001 Date: 04/12/2017 23:02:46*/SET NAMES utf8mb4;SET FOREIGN_KEY_CHECKS = 0;-- ------------------------------ Table structure for grade-- ----------------------------DROP TABLE IF EXISTS `grade`;CREATE TABLE `grade`  (  `grade_id` int(11) NOT NULL AUTO_INCREMENT,  `grade_name` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  PRIMARY KEY (`grade_id`) USING BTREE) ENGINE = InnoDB AUTO_INCREMENT = 8 CHARACTER SET = utf8 COLLATE = utf8_general_ci ROW_FORMAT = Compact;-- ------------------------------ Table structure for user-- ----------------------------DROP TABLE IF EXISTS `user`;CREATE TABLE `user`  (  `user_id` int(11) NOT NULL AUTO_INCREMENT,  `user_name` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `account` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `password` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `age` int(11) DEFAULT NULL,  `sex` int(11) DEFAULT NULL,  `card` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `tel` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `power` int(11) DEFAULT NULL,  `status` int(11) DEFAULT NULL,  PRIMARY KEY (`user_id`) USING BTREE) ENGINE = InnoDB AUTO_INCREMENT = 29 CHARACTER SET = utf8 COLLATE = utf8_general_ci ROW_FORMAT = Compact;-- ------------------------------ Table structure for vip-- ----------------------------DROP TABLE IF EXISTS `vip`;CREATE TABLE `vip`  (  `vip_id` int(11) NOT NULL AUTO_INCREMENT,  `vip_tel` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `vip_name` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `vip_sex` int(11) UNSIGNED ZEROFILL DEFAULT NULL,  `vip_address` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `vip_grade` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  `all_money` double(200, 2) DEFAULT NULL,  `vip_card` varchar(255) CHARACTER SET utf8 COLLATE utf8_general_ci DEFAULT NULL,  PRIMARY KEY (`vip_id`) USING BTREE) ENGINE = InnoDB AUTO_INCREMENT = 9 CHARACTER SET = utf8 COLLATE = utf8_general_ci ROW_FORMAT = Compact;SET FOREIGN_KEY_CHECKS = 1;```