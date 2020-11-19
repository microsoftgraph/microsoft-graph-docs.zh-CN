---
title: deviceManagementSettingDependency 资源类型
description: 设置的相关性信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76635e27bcb90eb393cfc2486f60c1a65315efb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268116"
---
# <a name="devicemanagementsettingdependency-resource-type"></a><span data-ttu-id="22034-103">deviceManagementSettingDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="22034-103">deviceManagementSettingDependency resource type</span></span>

<span data-ttu-id="22034-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22034-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22034-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22034-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22034-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22034-107">设置的相关性信息</span><span class="sxs-lookup"><span data-stu-id="22034-107">Dependency information for a setting</span></span>

## <a name="properties"></a><span data-ttu-id="22034-108">属性</span><span class="sxs-lookup"><span data-stu-id="22034-108">Properties</span></span>
|<span data-ttu-id="22034-109">属性</span><span class="sxs-lookup"><span data-stu-id="22034-109">Property</span></span>|<span data-ttu-id="22034-110">类型</span><span class="sxs-lookup"><span data-stu-id="22034-110">Type</span></span>|<span data-ttu-id="22034-111">说明</span><span class="sxs-lookup"><span data-stu-id="22034-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22034-112">definitionId</span><span class="sxs-lookup"><span data-stu-id="22034-112">definitionId</span></span>|<span data-ttu-id="22034-113">字符串</span><span class="sxs-lookup"><span data-stu-id="22034-113">String</span></span>|<span data-ttu-id="22034-114">设置的设置定义 ID 依赖于</span><span class="sxs-lookup"><span data-stu-id="22034-114">The setting definition ID of the setting depended on</span></span>|
|<span data-ttu-id="22034-115">施加</span><span class="sxs-lookup"><span data-stu-id="22034-115">constraints</span></span>|<span data-ttu-id="22034-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22034-116">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="22034-117">依赖项设置值的约束集合</span><span class="sxs-lookup"><span data-stu-id="22034-117">Collection of constraints for the dependency setting value</span></span>|

## <a name="relationships"></a><span data-ttu-id="22034-118">关系</span><span class="sxs-lookup"><span data-stu-id="22034-118">Relationships</span></span>
<span data-ttu-id="22034-119">无</span><span class="sxs-lookup"><span data-stu-id="22034-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22034-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22034-120">JSON Representation</span></span>
<span data-ttu-id="22034-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22034-121">Here is a JSON representation of the resource.</span></span>
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




