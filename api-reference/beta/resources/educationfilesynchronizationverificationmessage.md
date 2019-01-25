---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529892"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **类型** | string | 消息的类型。 可取值为：`error`、`warning`、`information`。 | 
| **fileName** | string | 包含错误的源文件。 |
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
