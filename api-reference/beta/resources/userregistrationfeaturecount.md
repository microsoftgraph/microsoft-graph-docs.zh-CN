---
title: userRegistrationFeatureCount 资源类型
description: 注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7c73d9cd17d5bf13eb5f8899e0d1e9dc6e27af67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132942"
---
# <a name="userregistrationfeaturecount-resource-type"></a>userRegistrationFeatureCount 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册或支持多重身份验证、密码重置和无Self-Service身份验证的用户数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|功能|authenticationMethodFeature|注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。 可取值为：`ssprRegistered`、`ssprEnabled`、`ssprCapable`、`passwordlessCapable`、`mfaCapable`。|
|userCount|Int64|用户数。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
