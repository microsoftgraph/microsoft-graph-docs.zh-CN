---
title: deviceManagementUserRightsSetting 资源类型
description: 代表设置用户权限。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b12dc0c1c682b59ef741b3d49083fd0739d27abb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844805"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="bec4a-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="bec4a-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="bec4a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bec4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bec4a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bec4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bec4a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bec4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bec4a-107">代表设置用户权限。</span><span class="sxs-lookup"><span data-stu-id="bec4a-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="bec4a-108">属性</span><span class="sxs-lookup"><span data-stu-id="bec4a-108">Properties</span></span>
|<span data-ttu-id="bec4a-109">属性</span><span class="sxs-lookup"><span data-stu-id="bec4a-109">Property</span></span>|<span data-ttu-id="bec4a-110">类型</span><span class="sxs-lookup"><span data-stu-id="bec4a-110">Type</span></span>|<span data-ttu-id="bec4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="bec4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bec4a-112">state</span><span class="sxs-lookup"><span data-stu-id="bec4a-112">state</span></span>|[<span data-ttu-id="bec4a-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="bec4a-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="bec4a-114">表示此用户的当前状态权限设置。</span><span class="sxs-lookup"><span data-stu-id="bec4a-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="bec4a-115">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="bec4a-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="bec4a-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="bec4a-116">localUsersOrGroups</span></span>|<span data-ttu-id="bec4a-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="bec4a-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="bec4a-118">表示本地用户或组如果允许此设置的状态，则将在设备上设置的集合。</span><span class="sxs-lookup"><span data-stu-id="bec4a-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="bec4a-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="bec4a-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bec4a-120">关系</span><span class="sxs-lookup"><span data-stu-id="bec4a-120">Relationships</span></span>
<span data-ttu-id="bec4a-121">无</span><span class="sxs-lookup"><span data-stu-id="bec4a-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bec4a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bec4a-122">JSON Representation</span></span>
<span data-ttu-id="bec4a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bec4a-123">Here is a JSON representation of the resource.</span></span>
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





