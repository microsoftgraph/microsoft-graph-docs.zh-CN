---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: firewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a7dab6f20198a8e0ebe97546c797515342af5b29
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60451442"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>firewallPreSharedKeyEncodingMethodType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallPreSharedKeyEncodingMethod 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|无|1|预共享密钥未进行编码。 相反，它保留为宽字符格式|
|utF8|2|使用 UTF-8 对预共享密钥进行编码|



