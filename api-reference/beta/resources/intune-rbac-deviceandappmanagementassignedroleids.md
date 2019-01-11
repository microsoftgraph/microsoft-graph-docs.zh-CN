---
title: deviceAndAppManagementAssignedRoleIds 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1ae87f1a8430ef2539fe10e813390b0fbd68b267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846338"
---
# <a name="deviceandappmanagementassignedroleids-resource-type"></a><span data-ttu-id="9ccb8-103">deviceAndAppManagementAssignedRoleIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ccb8-103">deviceAndAppManagementAssignedRoleIds resource type</span></span>

> <span data-ttu-id="9ccb8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ccb8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ccb8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ccb8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9ccb8-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9ccb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ccb8-108">Properties</span></span>
|<span data-ttu-id="9ccb8-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ccb8-109">Property</span></span>|<span data-ttu-id="9ccb8-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ccb8-110">Type</span></span>|<span data-ttu-id="9ccb8-111">Description</span><span class="sxs-lookup"><span data-stu-id="9ccb8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ccb8-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="9ccb8-112">roleDefinitionIds</span></span>|<span data-ttu-id="9ccb8-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="9ccb8-113">Guid collection</span></span>|<span data-ttu-id="9ccb8-114">特定分配给用户的角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="9ccb8-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="9ccb8-115">roleAssignmentIds</span></span>|<span data-ttu-id="9ccb8-116">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="9ccb8-116">Guid collection</span></span>|<span data-ttu-id="9ccb8-117">特定分配给用户的角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ccb8-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="9ccb8-118">Relationships</span></span>
<span data-ttu-id="9ccb8-119">无</span><span class="sxs-lookup"><span data-stu-id="9ccb8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ccb8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ccb8-120">JSON Representation</span></span>
<span data-ttu-id="9ccb8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ccb8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleIds",
  "roleDefinitionIds": [
    "Guid"
  ],
  "roleAssignmentIds": [
    "Guid"
  ]
}
```





