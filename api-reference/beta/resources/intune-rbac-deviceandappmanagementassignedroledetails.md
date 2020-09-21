---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9dff637f950d980b3fc0de89ecfde26da6b40de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070798"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="270c4-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="270c4-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="270c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="270c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="270c4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="270c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="270c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="270c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="270c4-107">分配给用户的角色定义和角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="270c4-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="270c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="270c4-108">Properties</span></span>
|<span data-ttu-id="270c4-109">属性</span><span class="sxs-lookup"><span data-stu-id="270c4-109">Property</span></span>|<span data-ttu-id="270c4-110">类型</span><span class="sxs-lookup"><span data-stu-id="270c4-110">Type</span></span>|<span data-ttu-id="270c4-111">说明</span><span class="sxs-lookup"><span data-stu-id="270c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270c4-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="270c4-112">roleDefinitionIds</span></span>|<span data-ttu-id="270c4-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="270c4-113">String collection</span></span>|<span data-ttu-id="270c4-114">分配给用户的表列角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="270c4-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="270c4-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="270c4-115">roleAssignmentIds</span></span>|<span data-ttu-id="270c4-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="270c4-116">String collection</span></span>|<span data-ttu-id="270c4-117">分配给用户的表列角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="270c4-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270c4-118">关系</span><span class="sxs-lookup"><span data-stu-id="270c4-118">Relationships</span></span>
<span data-ttu-id="270c4-119">无</span><span class="sxs-lookup"><span data-stu-id="270c4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="270c4-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="270c4-120">JSON Representation</span></span>
<span data-ttu-id="270c4-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="270c4-121">Here is a JSON representation of the resource.</span></span>
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






