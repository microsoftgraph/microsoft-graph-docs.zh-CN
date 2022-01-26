---
title: 同步资源类型
description: 表示通过 Microsoft Azure Active Directory (Azure AD) API 执行标识Graph的功能。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 9fd52e5fde2a3eee110709d0817930c0a017ee7e
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226293"
---
# <a name="synchronization-resource-type"></a>同步资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示通过 Microsoft Azure Active Directory (Azure AD) API 执行标识Graph的功能。 标识 (也称为预配 *) ，* 允许你将 (创建、维护) 和取消预配 (删除) 用户标识和角色从 Azure AD 自动删除到支持的云应用程序。 有关详细信息，请参阅应用程序[预配在应用程序中Azure Active Directory](/azure/active-directory/app-provisioning/how-provisioning-works)

## <a name="methods"></a>方法


|方法|返回类型|说明|
|:---|:---|:---|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|无| 获取 OAuth 访问令牌，以授权Azure AD预配服务将用户预配到应用程序中。 |
|[添加密码](../api/synchronization-synchronization-secrets.md)|无| 提供用于与目标系统建立连接的凭据。 |

<!--
|Method|Return type|Description|
|:---|:---|:---|
|[List synchronizations](../api/synchronization-synchronization-list.md)|[synchronization](../resources/synchronization-synchronization.md) collection|Get a list of the [synchronization](../resources/synchronization-synchronization.md) objects and their properties.|
|[Create synchronization](../api/synchronization-serviceprincipal-post-synchronization.md)|[synchronization](../resources/synchronization-synchronization.md)|Create a new [synchronization](../resources/synchronization-synchronization.md) object.|
|[Get synchronization](../api/synchronization-synchronization-get.md)|[synchronization](../resources/synchronization-synchronization.md)|Read the properties and relationships of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Update synchronization](../api/synchronization-synchronization-update.md)|[synchronization](../resources/synchronization-synchronization.md)|Update the properties of a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Delete synchronization](../api/synchronization-synchronization-delete.md)|None|Deletes a [synchronization](../resources/synchronization-synchronization.md) object.|
|[Ping](../api/synchronization-synchronization-ping.md)|String|**TODO: Add Description**|
|[acquireAccessToken](../api/synchronization-synchronization-acquireaccesstoken.md)|None|**TODO: Add Description**|
|[List jobs](../api/synchronization-synchronization-list-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md) collection|Get the synchronizationJob resources from the jobs navigation property.|
|[Create synchronizationJob](../api/synchronization-synchronization-post-jobs.md)|[synchronizationJob](../resources/synchronization-synchronizationjob.md)|Create a new synchronizationJob object.|
|[List templates](../api/synchronization-synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) collection|Get the synchronizationTemplate resources from the templates navigation property.|
|[Create synchronizationTemplate](../api/synchronization-synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md)|Create a new synchronizationTemplate object.|
-->

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|secrets|[synchronizationSecretKeyStringValuePair](synchronization-synchronizationsecretkeystringvaluepair.md) 集合| 表示用于访问预配的云应用程序的凭据集合。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|jobs|[synchronizationJob](../resources/synchronization-synchronizationjob.md) 集合| 通过定期在后台运行、轮询一个目录中的更改，将它们推送到另一个目录执行同步。|
|模板|[synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) 集合| 为特定应用程序预配置的同步设置。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronization",
  "version": "String",
  "secrets": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```

