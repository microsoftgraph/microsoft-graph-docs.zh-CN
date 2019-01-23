---
title: deviceManagementUserRightsSetting 资源类型
description: 代表设置用户权限。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35e6ec1a5faa5556a0e113df145d718c488b1669
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415052"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="59083-103">deviceManagementUserRightsSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="59083-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="59083-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="59083-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59083-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59083-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59083-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59083-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59083-107">代表设置用户权限。</span><span class="sxs-lookup"><span data-stu-id="59083-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="59083-108">属性</span><span class="sxs-lookup"><span data-stu-id="59083-108">Properties</span></span>
|<span data-ttu-id="59083-109">属性</span><span class="sxs-lookup"><span data-stu-id="59083-109">Property</span></span>|<span data-ttu-id="59083-110">类型</span><span class="sxs-lookup"><span data-stu-id="59083-110">Type</span></span>|<span data-ttu-id="59083-111">说明</span><span class="sxs-lookup"><span data-stu-id="59083-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59083-112">state</span><span class="sxs-lookup"><span data-stu-id="59083-112">state</span></span>|[<span data-ttu-id="59083-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="59083-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="59083-114">表示此用户的当前状态权限设置。</span><span class="sxs-lookup"><span data-stu-id="59083-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="59083-115">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="59083-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="59083-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="59083-116">localUsersOrGroups</span></span>|<span data-ttu-id="59083-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)集合</span><span class="sxs-lookup"><span data-stu-id="59083-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="59083-118">表示本地用户或组如果允许此设置的状态，则将在设备上设置的集合。</span><span class="sxs-lookup"><span data-stu-id="59083-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="59083-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="59083-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59083-120">关系</span><span class="sxs-lookup"><span data-stu-id="59083-120">Relationships</span></span>
<span data-ttu-id="59083-121">无</span><span class="sxs-lookup"><span data-stu-id="59083-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59083-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59083-122">JSON Representation</span></span>
<span data-ttu-id="59083-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59083-123">Here is a JSON representation of the resource.</span></span>
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




