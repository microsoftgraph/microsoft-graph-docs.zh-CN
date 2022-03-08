---
title: azureAdTokenAuthentication 资源类型
description: 定义用于Azure AD自定义访问包工作流扩展进行身份验证的客户端应用程序。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e1161897cf09ae1ad25d312b8ba5ca2bdf31617
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338299"
---
# <a name="azureadtokenauthentication-resource-type"></a>azureAdTokenAuthentication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义用于Azure AD访问包工作流扩展对逻辑应用进行身份验证[的客户端应用程序](customaccesspackageworkflowextension.md)。 只需要应用程序的应用程序 ID。 派生自 [customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|resourceId|String|要用于对逻辑应用Azure AD自定义访问包工作流扩展进行身份验证的客户端应用程序的 **appID**。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.azureAdTokenAuthentication",
  "baseType": "microsoft.graph.customExtensionAuthenticationConfiguration"
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
  "resourceId": "String" 
 } 
```
