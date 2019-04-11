---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93f99cdc91d046b9ebf292bbd34f1bba39b494ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771402"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="bf745-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf745-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="bf745-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf745-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf745-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf745-106">分配给用户的角色定义和角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="bf745-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="bf745-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf745-107">Properties</span></span>
|<span data-ttu-id="bf745-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf745-108">Property</span></span>|<span data-ttu-id="bf745-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf745-109">Type</span></span>|<span data-ttu-id="bf745-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf745-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf745-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="bf745-111">roleDefinitionIds</span></span>|<span data-ttu-id="bf745-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="bf745-112">String collection</span></span>|<span data-ttu-id="bf745-113">分配给用户的表列角色定义的角色定义 id。</span><span class="sxs-lookup"><span data-stu-id="bf745-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="bf745-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="bf745-114">roleAssignmentIds</span></span>|<span data-ttu-id="bf745-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="bf745-115">String collection</span></span>|<span data-ttu-id="bf745-116">分配给用户的表列角色分配的角色分配 id。</span><span class="sxs-lookup"><span data-stu-id="bf745-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf745-117">关系</span><span class="sxs-lookup"><span data-stu-id="bf745-117">Relationships</span></span>
<span data-ttu-id="bf745-118">无</span><span class="sxs-lookup"><span data-stu-id="bf745-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf745-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf745-119">JSON Representation</span></span>
<span data-ttu-id="bf745-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf745-120">Here is a JSON representation of the resource.</span></span>
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





