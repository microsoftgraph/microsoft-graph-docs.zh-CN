---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1590470f436dac6572ebf9d0430d144060f9b7f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773943"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="df8b8-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="df8b8-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="df8b8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df8b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df8b8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df8b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df8b8-106">分配给用户的角色定义和角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="df8b8-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="df8b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="df8b8-107">Properties</span></span>
|<span data-ttu-id="df8b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="df8b8-108">Property</span></span>|<span data-ttu-id="df8b8-109">类型</span><span class="sxs-lookup"><span data-stu-id="df8b8-109">Type</span></span>|<span data-ttu-id="df8b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="df8b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df8b8-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="df8b8-111">roleDefinitionIds</span></span>|<span data-ttu-id="df8b8-112">String collection</span><span class="sxs-lookup"><span data-stu-id="df8b8-112">String collection</span></span>|<span data-ttu-id="df8b8-113">分配给用户的表列角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="df8b8-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="df8b8-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="df8b8-114">roleAssignmentIds</span></span>|<span data-ttu-id="df8b8-115">String collection</span><span class="sxs-lookup"><span data-stu-id="df8b8-115">String collection</span></span>|<span data-ttu-id="df8b8-116">分配给用户的表列角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="df8b8-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df8b8-117">关系</span><span class="sxs-lookup"><span data-stu-id="df8b8-117">Relationships</span></span>
<span data-ttu-id="df8b8-118">无</span><span class="sxs-lookup"><span data-stu-id="df8b8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df8b8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df8b8-119">JSON Representation</span></span>
<span data-ttu-id="df8b8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df8b8-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```



