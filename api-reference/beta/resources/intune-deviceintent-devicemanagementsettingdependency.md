---
title: deviceManagementSettingDependency 资源类型
description: 设置的相关性信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9cb6abb17963a9c22e027a4ba56eadfd3b07f6a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525255"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="19406-103">deviceManagementSettingDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="19406-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="19406-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="19406-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19406-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19406-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19406-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19406-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19406-107">设置的相关性信息</span><span class="sxs-lookup"><span data-stu-id="19406-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="19406-108">属性</span><span class="sxs-lookup"><span data-stu-id="19406-108">Properties</span></span>
|<span data-ttu-id="19406-109">属性</span><span class="sxs-lookup"><span data-stu-id="19406-109">Property</span></span>|<span data-ttu-id="19406-110">类型</span><span class="sxs-lookup"><span data-stu-id="19406-110">Type</span></span>|<span data-ttu-id="19406-111">说明</span><span class="sxs-lookup"><span data-stu-id="19406-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19406-112">definitionId</span><span class="sxs-lookup"><span data-stu-id="19406-112">definitionId</span></span>|<span data-ttu-id="19406-113">String</span><span class="sxs-lookup"><span data-stu-id="19406-113">String</span></span>|<span data-ttu-id="19406-114">设置的设置定义 ID 依赖于</span><span class="sxs-lookup"><span data-stu-id="19406-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="19406-115">施加</span><span class="sxs-lookup"><span data-stu-id="19406-115">constraints</span></span>|<span data-ttu-id="19406-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)集合</span><span class="sxs-lookup"><span data-stu-id="19406-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="19406-117">依赖项设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="19406-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="19406-118">关系</span><span class="sxs-lookup"><span data-stu-id="19406-118">Relationships</span></span>
<span data-ttu-id="19406-119">无</span><span class="sxs-lookup"><span data-stu-id="19406-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19406-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19406-120">JSON Representation</span></span>
<span data-ttu-id="19406-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19406-121">Here is a JSON representation of the resource.</span></span>
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



