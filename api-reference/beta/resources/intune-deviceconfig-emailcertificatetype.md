---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a2ba44ebc301e0d225ae5353059378cdbcbed91
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787860"
---
# <a name="emailcertificatetype-enum-type"></a>emailCertificateType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

支持的电子邮件签名和加密的证书源。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|请勿将证书用作源。|
|证书|1|将证书用于证书源。|
|derivedCredential|2|对证书源使用派生凭据。|



