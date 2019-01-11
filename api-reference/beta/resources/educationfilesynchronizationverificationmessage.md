---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845512"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **类型** | string | 消息的类型。 可取值为：`error`、`warning`、`information`。 | 
| **文件名** | string | 包含错误的源文件。 |
| **说明** | string | 有关邮件类型的详细的信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
