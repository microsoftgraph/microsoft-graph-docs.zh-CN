---
title: deviceManagementUserRightsSetting 资源类型
description: 代表用户权限设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b83e7c1c1c7409801b8ba79db2af6e4f167d0fd7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968463"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="3c934-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c934-103">deviceManagementUserRightsSetting resource type</span></span>

<span data-ttu-id="3c934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c934-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c934-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c934-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c934-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c934-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c934-107">代表用户权限设置。</span><span class="sxs-lookup"><span data-stu-id="3c934-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="3c934-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c934-108">Properties</span></span>
|<span data-ttu-id="3c934-109">属性</span><span class="sxs-lookup"><span data-stu-id="3c934-109">Property</span></span>|<span data-ttu-id="3c934-110">类型</span><span class="sxs-lookup"><span data-stu-id="3c934-110">Type</span></span>|<span data-ttu-id="3c934-111">说明</span><span class="sxs-lookup"><span data-stu-id="3c934-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c934-112">state</span><span class="sxs-lookup"><span data-stu-id="3c934-112">state</span></span>|[<span data-ttu-id="3c934-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="3c934-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="3c934-114">表示此用户权限设置的当前状态。</span><span class="sxs-lookup"><span data-stu-id="3c934-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="3c934-115">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3c934-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="3c934-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="3c934-116">localUsersOrGroups</span></span>|<span data-ttu-id="3c934-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3c934-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="3c934-118">表示将在设备上设置的本地用户或组的集合（如果允许此设置的状态）。</span><span class="sxs-lookup"><span data-stu-id="3c934-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="3c934-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3c934-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c934-120">关系</span><span class="sxs-lookup"><span data-stu-id="3c934-120">Relationships</span></span>
<span data-ttu-id="3c934-121">无</span><span class="sxs-lookup"><span data-stu-id="3c934-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c934-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c934-122">JSON Representation</span></span>
<span data-ttu-id="3c934-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c934-123">Here is a JSON representation of the resource.</span></span>
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






