---
title: userRegistrationFeatureCount 资源类型
description: 注册或支持多重身份验证、Self-Service密码重置和无密码身份验证的用户数。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 609c8d30547093c19d93428a0c779687b93ae018
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820160"
---
# <a name="userregistrationfeaturecount-resource-type"></a>userRegistrationFeatureCount 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示注册或能够进行多重身份验证、Self-Service密码重置和无密码身份验证的用户数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|特征|authenticationMethodFeature|注册或支持多重身份验证、Self-Service密码重置和无密码身份验证的用户数。 可取值为：`ssprRegistered`、`ssprEnabled`、`ssprCapable`、`passwordlessCapable`、`mfaCapable`。|
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
