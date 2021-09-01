---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f6e7635a8893559d4f86f60210aba3b9f08d68b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58778743"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书吊销状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未撤销。|
|pending|1|吊销挂起。|
|issued|2|颁发的吊销命令。|
|failed|3|吊销失败。|
|revoked|4 |已吊销。|



