---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: firewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36810f72095d955b40e6e1c288f8d175d24de88b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075471"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallCertificateRevocationListCheckMethod 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|无|1|不检查证书吊销列表|
|attempt|2|仅在检查确认证书时，才尝试 CRL 检查并允许证书|
|require|3|在允许证书之前需要成功的 CRL 检查|



