---
title: customAccessPackageWorkflowExtension 资源类型
description: 定义逻辑应用的属性，可在访问包请求和分配周期的各个阶段调用这些属性。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b89d41ec573d6035e19590d7015df4e7269909f3
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672733"
---
# <a name="customaccesspackageworkflowextension-resource-type"></a>customAccessPackageWorkflowExtension 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义逻辑应用的属性，可在访问包请求和分配周期的各个阶段调用这些属性。 可以将逻辑应用与权利管理集成，以扩大核心权利管理用例之外的治理工作流。 可以使用此工作流将以下用例与逻辑应用集成：
- 请求 [访问包时](accesspackageassignmentrequest.md)
- 授予 [访问包请求时](accesspackageassignment.md)
- 访问 [包分配过期时](accesspackageassignment.md)

继承并派生自 [customCalloutExtension](../resources/customcalloutextension.md)。


## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-list-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 集合|获取 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象及其属性的列表。|
|[Create customAccessPackageWorkflowExtensions](../api/accesspackagecatalog-post-customaccesspackageworkflowextensions.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|创建新的 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。|
|[获取 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-get.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|读取 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象的属性和关系。|
|[更新 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-update.md)|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|更新 [customAccessPackageWorkflowExtension 对象](../resources/customaccesspackageworkflowextension.md) 的属性。|
|[删除 customAccessPackageWorkflowExtension](../api/customaccesspackageworkflowextension-delete.md)|无|删除 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|用于保护对逻辑应用的 API 调用的配置。 例如，使用 OAuth 客户端凭据流。 继承自 [customCalloutExtension](../resources/customcalloutextension.md)。|
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| HTTP 连接设置，用于定义Azure AD逻辑应用的连接可以等待的时间、可以重试的退出连接多少次以及允许重试时出现异常情况。 继承自 [customCalloutExtension](../resources/customcalloutextension.md)。|
|createdDateTime|DateTimeOffset|表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|
|说明|String|customAccessPackageWorkflowExtension 对象的说明。 继承自 [customCalloutExtension](../resources/customcalloutextension.md)。 只读。|
|displayName|String|customAccessPackageWorkflowExtension 对象的显示名称。 继承自 [customCalloutExtension](../resources/customcalloutextension.md)。 只读。 支持 `$filter`（`contains`）。|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|用于配置终结点以调用逻辑应用的工作流的类型和详细信息。 继承自 [customCalloutExtension](../resources/customcalloutextension.md)。|  
|id|String|customAccessPackageWorkflowExtension 对象的标识符。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customAccessPackageWorkflowExtension",
  "baseType": "microsoft.graph.customCalloutExtension",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customAccessPackageWorkflowExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  },
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  }
}
```
