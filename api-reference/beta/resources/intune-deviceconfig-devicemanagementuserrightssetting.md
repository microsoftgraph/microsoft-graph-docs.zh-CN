---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f8fd9d2217fd39c4d2dc8e9db28cb5b5dcd0a1e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172182"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="66cf2-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="66cf2-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="66cf2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66cf2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66cf2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66cf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66cf2-106">代表用户权限设置。</span><span class="sxs-lookup"><span data-stu-id="66cf2-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="66cf2-107">属性</span><span class="sxs-lookup"><span data-stu-id="66cf2-107">Properties</span></span>
|<span data-ttu-id="66cf2-108">属性</span><span class="sxs-lookup"><span data-stu-id="66cf2-108">Property</span></span>|<span data-ttu-id="66cf2-109">类型</span><span class="sxs-lookup"><span data-stu-id="66cf2-109">Type</span></span>|<span data-ttu-id="66cf2-110">说明</span><span class="sxs-lookup"><span data-stu-id="66cf2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66cf2-111">state</span><span class="sxs-lookup"><span data-stu-id="66cf2-111">state</span></span>|[<span data-ttu-id="66cf2-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="66cf2-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="66cf2-113">表示此用户权限设置的当前状态。</span><span class="sxs-lookup"><span data-stu-id="66cf2-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="66cf2-114">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="66cf2-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="66cf2-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="66cf2-115">localUsersOrGroups</span></span>|<span data-ttu-id="66cf2-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="66cf2-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="66cf2-117">表示将在设备上设置的本地用户或组的集合 (如果允许此设置的状态)。</span><span class="sxs-lookup"><span data-stu-id="66cf2-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="66cf2-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="66cf2-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66cf2-119">关系</span><span class="sxs-lookup"><span data-stu-id="66cf2-119">Relationships</span></span>
<span data-ttu-id="66cf2-120">无</span><span class="sxs-lookup"><span data-stu-id="66cf2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66cf2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66cf2-121">JSON Representation</span></span>
<span data-ttu-id="66cf2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66cf2-122">Here is a JSON representation of the resource.</span></span>
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




