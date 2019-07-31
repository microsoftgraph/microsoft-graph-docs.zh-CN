---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e041966f141ada4ca584d1c90cf9e1bd1af1f108
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001570"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="af715-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="af715-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="af715-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af715-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af715-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af715-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af715-106">代表用户权限设置。</span><span class="sxs-lookup"><span data-stu-id="af715-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="af715-107">属性</span><span class="sxs-lookup"><span data-stu-id="af715-107">Properties</span></span>
|<span data-ttu-id="af715-108">属性</span><span class="sxs-lookup"><span data-stu-id="af715-108">Property</span></span>|<span data-ttu-id="af715-109">类型</span><span class="sxs-lookup"><span data-stu-id="af715-109">Type</span></span>|<span data-ttu-id="af715-110">说明</span><span class="sxs-lookup"><span data-stu-id="af715-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af715-111">state</span><span class="sxs-lookup"><span data-stu-id="af715-111">state</span></span>|[<span data-ttu-id="af715-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="af715-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="af715-113">表示此用户权限设置的当前状态。</span><span class="sxs-lookup"><span data-stu-id="af715-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="af715-114">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="af715-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="af715-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="af715-115">localUsersOrGroups</span></span>|<span data-ttu-id="af715-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="af715-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="af715-117">表示将在设备上设置的本地用户或组的集合 (如果允许此设置的状态)。</span><span class="sxs-lookup"><span data-stu-id="af715-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="af715-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="af715-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af715-119">关系</span><span class="sxs-lookup"><span data-stu-id="af715-119">Relationships</span></span>
<span data-ttu-id="af715-120">无</span><span class="sxs-lookup"><span data-stu-id="af715-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af715-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af715-121">JSON Representation</span></span>
<span data-ttu-id="af715-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af715-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```





