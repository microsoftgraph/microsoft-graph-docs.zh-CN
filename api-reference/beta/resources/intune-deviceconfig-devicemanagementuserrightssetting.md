---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2228e28b2edb3584a0861628644188d6fd54495b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802623"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="90c53-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="90c53-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="90c53-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90c53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90c53-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90c53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c53-106">代表用户权限设置。</span><span class="sxs-lookup"><span data-stu-id="90c53-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="90c53-107">属性</span><span class="sxs-lookup"><span data-stu-id="90c53-107">Properties</span></span>
|<span data-ttu-id="90c53-108">属性</span><span class="sxs-lookup"><span data-stu-id="90c53-108">Property</span></span>|<span data-ttu-id="90c53-109">类型</span><span class="sxs-lookup"><span data-stu-id="90c53-109">Type</span></span>|<span data-ttu-id="90c53-110">说明</span><span class="sxs-lookup"><span data-stu-id="90c53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90c53-111">state</span><span class="sxs-lookup"><span data-stu-id="90c53-111">state</span></span>|[<span data-ttu-id="90c53-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="90c53-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="90c53-113">表示此用户权限设置的当前状态。</span><span class="sxs-lookup"><span data-stu-id="90c53-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="90c53-114">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="90c53-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="90c53-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="90c53-115">localUsersOrGroups</span></span>|<span data-ttu-id="90c53-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="90c53-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="90c53-117">表示将在设备上设置的本地用户或组的集合 (如果允许此设置的状态)。</span><span class="sxs-lookup"><span data-stu-id="90c53-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="90c53-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="90c53-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90c53-119">关系</span><span class="sxs-lookup"><span data-stu-id="90c53-119">Relationships</span></span>
<span data-ttu-id="90c53-120">无</span><span class="sxs-lookup"><span data-stu-id="90c53-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90c53-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90c53-121">JSON Representation</span></span>
<span data-ttu-id="90c53-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90c53-122">Here is a JSON representation of the resource.</span></span>
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





