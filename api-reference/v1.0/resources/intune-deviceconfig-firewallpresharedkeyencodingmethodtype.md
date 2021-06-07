---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: firewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 200177be7f8258965067f12cace3b163aefc6b78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755054"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>firewallPreSharedKeyEncodingMethodType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallPreSharedKeyEncodingMethod 的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|无|1|预共享密钥未进行编码。 相反，它保留为宽字符格式|
|utF8|2|使用 UTF-8 对预共享密钥进行编码|




