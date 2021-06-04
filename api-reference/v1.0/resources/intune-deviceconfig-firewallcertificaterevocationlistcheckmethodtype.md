---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: firewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 779cfe8b8576d475df62ed112709aa0c2e9b6c63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754725"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallCertificateRevocationListCheckMethod 的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|无|1|不检查证书吊销列表|
|attempt|2|仅在检查确认证书时，才尝试 CRL 检查并允许证书|
|require|3|在允许证书之前需要成功的 CRL 检查|




