---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 013de6921453a474f221e7139b2d04fa86f37926
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791994"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="45926-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="45926-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="45926-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45926-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45926-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45926-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45926-106">代表用户权限设置。</span><span class="sxs-lookup"><span data-stu-id="45926-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="45926-107">属性</span><span class="sxs-lookup"><span data-stu-id="45926-107">Properties</span></span>
|<span data-ttu-id="45926-108">属性</span><span class="sxs-lookup"><span data-stu-id="45926-108">Property</span></span>|<span data-ttu-id="45926-109">类型</span><span class="sxs-lookup"><span data-stu-id="45926-109">Type</span></span>|<span data-ttu-id="45926-110">说明</span><span class="sxs-lookup"><span data-stu-id="45926-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45926-111">state</span><span class="sxs-lookup"><span data-stu-id="45926-111">state</span></span>|[<span data-ttu-id="45926-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="45926-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="45926-113">表示此用户权限设置的当前状态。</span><span class="sxs-lookup"><span data-stu-id="45926-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="45926-114">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="45926-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="45926-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="45926-115">localUsersOrGroups</span></span>|<span data-ttu-id="45926-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="45926-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="45926-117">表示将在设备上设置的本地用户或组的集合（如果允许此设置的状态）。</span><span class="sxs-lookup"><span data-stu-id="45926-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="45926-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="45926-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45926-119">关系</span><span class="sxs-lookup"><span data-stu-id="45926-119">Relationships</span></span>
<span data-ttu-id="45926-120">无</span><span class="sxs-lookup"><span data-stu-id="45926-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45926-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45926-121">JSON Representation</span></span>
<span data-ttu-id="45926-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45926-122">Here is a JSON representation of the resource.</span></span>
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



