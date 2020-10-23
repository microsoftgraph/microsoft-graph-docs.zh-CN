---
title: deviceManagementSettingDependency 资源类型
description: 设置的相关性信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06681607295f9cee22c67f74339a8b99381b89a2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724507"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="31ab9-103">deviceManagementSettingDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="31ab9-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="31ab9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31ab9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31ab9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="31ab9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31ab9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31ab9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31ab9-107">设置的相关性信息</span><span class="sxs-lookup"><span data-stu-id="31ab9-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="31ab9-108">属性</span><span class="sxs-lookup"><span data-stu-id="31ab9-108">Properties</span></span>
|<span data-ttu-id="31ab9-109">属性</span><span class="sxs-lookup"><span data-stu-id="31ab9-109">Property</span></span>|<span data-ttu-id="31ab9-110">类型</span><span class="sxs-lookup"><span data-stu-id="31ab9-110">Type</span></span>|<span data-ttu-id="31ab9-111">说明</span><span class="sxs-lookup"><span data-stu-id="31ab9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ab9-112">definitionId</span><span class="sxs-lookup"><span data-stu-id="31ab9-112">definitionId</span></span>|<span data-ttu-id="31ab9-113">String</span><span class="sxs-lookup"><span data-stu-id="31ab9-113">String</span></span>|<span data-ttu-id="31ab9-114">设置的设置定义 ID 依赖于</span><span class="sxs-lookup"><span data-stu-id="31ab9-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="31ab9-115">施加</span><span class="sxs-lookup"><span data-stu-id="31ab9-115">constraints</span></span>|<span data-ttu-id="31ab9-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31ab9-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="31ab9-117">依赖项设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="31ab9-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="31ab9-118">关系</span><span class="sxs-lookup"><span data-stu-id="31ab9-118">Relationships</span></span>
<span data-ttu-id="31ab9-119">无</span><span class="sxs-lookup"><span data-stu-id="31ab9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31ab9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31ab9-120">JSON Representation</span></span>
<span data-ttu-id="31ab9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31ab9-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
      "supportedTypes": [
        "String"
      ]
    }
  ]
}
```





