---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: firewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4cc592c2213cef70af497c9f3f4779bcae88e5694599a5d0f3fff50ac7d8b56e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189581"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallCertificateRevocationListCheckMethod 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|无|1|不检查证书吊销列表|
|attempt|2|仅在检查确认证书时，才尝试 CRL 检查并允许证书|
|require|3|在允许证书之前需要成功的 CRL 检查|




