---
title: deviceManagementSettingDependency 资源类型
description: 设置的相关性信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 100a6d441e161c353425f2d890e9468ebb32f3e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364661"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="acff7-103">deviceManagementSettingDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="acff7-103">deviceManagementSettingDependency resource type</span></span>

> <span data-ttu-id="acff7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="acff7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acff7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acff7-106">设置的相关性信息</span><span class="sxs-lookup"><span data-stu-id="acff7-106">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="acff7-107">属性</span><span class="sxs-lookup"><span data-stu-id="acff7-107">Properties</span></span>
|<span data-ttu-id="acff7-108">属性</span><span class="sxs-lookup"><span data-stu-id="acff7-108">Property</span></span>|<span data-ttu-id="acff7-109">类型</span><span class="sxs-lookup"><span data-stu-id="acff7-109">Type</span></span>|<span data-ttu-id="acff7-110">说明</span><span class="sxs-lookup"><span data-stu-id="acff7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acff7-111">definitionId</span><span class="sxs-lookup"><span data-stu-id="acff7-111">definitionId</span></span>|<span data-ttu-id="acff7-112">String</span><span class="sxs-lookup"><span data-stu-id="acff7-112">String</span></span>|<span data-ttu-id="acff7-113">设置的设置定义 ID 依赖于</span><span class="sxs-lookup"><span data-stu-id="acff7-113">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="acff7-114">施加</span><span class="sxs-lookup"><span data-stu-id="acff7-114">constraints</span></span>|<span data-ttu-id="acff7-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="acff7-115">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="acff7-116">依赖项设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="acff7-116">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="acff7-117">关系</span><span class="sxs-lookup"><span data-stu-id="acff7-117">Relationships</span></span>
<span data-ttu-id="acff7-118">无</span><span class="sxs-lookup"><span data-stu-id="acff7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acff7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acff7-119">JSON Representation</span></span>
<span data-ttu-id="acff7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acff7-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```



