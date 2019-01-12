---
title: deviceManagementUserRightsSetting 资源类型
description: 代表设置用户权限。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 889ce941037013cb66134f9c78aa18fb90aed29a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931746"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="8e358-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e358-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="8e358-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e358-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e358-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e358-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e358-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8e358-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e358-107">代表设置用户权限。</span><span class="sxs-lookup"><span data-stu-id="8e358-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="8e358-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e358-108">Properties</span></span>
|<span data-ttu-id="8e358-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e358-109">Property</span></span>|<span data-ttu-id="8e358-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e358-110">Type</span></span>|<span data-ttu-id="8e358-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e358-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e358-112">state</span><span class="sxs-lookup"><span data-stu-id="8e358-112">state</span></span>|[<span data-ttu-id="8e358-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8e358-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="8e358-114">表示此用户的当前状态权限设置。</span><span class="sxs-lookup"><span data-stu-id="8e358-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="8e358-115">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="8e358-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8e358-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="8e358-116">localUsersOrGroups</span></span>|<span data-ttu-id="8e358-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="8e358-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="8e358-118">表示本地用户或组如果允许此设置的状态，则将在设备上设置的集合。</span><span class="sxs-lookup"><span data-stu-id="8e358-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="8e358-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8e358-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e358-120">关系</span><span class="sxs-lookup"><span data-stu-id="8e358-120">Relationships</span></span>
<span data-ttu-id="8e358-121">无</span><span class="sxs-lookup"><span data-stu-id="8e358-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e358-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e358-122">JSON Representation</span></span>
<span data-ttu-id="8e358-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e358-123">Here is a JSON representation of the resource.</span></span>
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





