---
title: userFlowApiConnectorConfiguration 资源类型
description: 表示为用户流启用的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78e93f4b743f57a68faad530f2a26ad6dead8a08
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292884"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>userFlowApiConnectorConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义在用户流中的特定点调用哪些 API。  此对象的每个关系对应于用户流中可配置为调用 API 连接器的特定步骤。

## <a name="relationships"></a>关系

| 关系            | 类型                                            | 说明                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | 指定在用户注册 (时完成与外部标识提供程序 (如 Google、Facebook 或 Azure AD) 的联盟后要调用的 API (不适用于登录) 。 |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | 指定在用户提交收集的属性后以及注册期间创建用户之前要调用的 API。                                                      |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
