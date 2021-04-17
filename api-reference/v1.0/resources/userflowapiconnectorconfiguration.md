---
title: userFlowApiConnectorConfiguration 资源类型
description: 表示为用户流启用的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b9d9b87bf59a796e8c79875a8506fccdd4d3447b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882943"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a>userFlowApiConnectorConfiguration 资源类型

命名空间：microsoft.graph

定义在用户流中的特定点调用的 API。  此对象的每个关系对应于可配置为调用 API 连接器的用户流中的特定步骤。

## <a name="relationships"></a>关系

| 关系            | 类型                                            | 说明                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| postFederationSignup    | [identityApiConnector](identityapiconnector.md) | 指定与外部标识提供程序建立联盟后要调用的 API。 例如，当用户注册 Google、Facebook 或 Azure AD API 时， (不适用于登录帐户) 。 |
| postAttributeCollection | [identityApiConnector](identityapiconnector.md) | 指定在用户提交收集的属性后以及注册期间创建用户帐户之前要调用的 API。                                                      |

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
