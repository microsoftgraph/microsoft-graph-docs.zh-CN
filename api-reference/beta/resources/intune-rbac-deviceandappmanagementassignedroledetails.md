---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03b98e2d98774ae166bba6b9ab74d8e42953c78e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940027"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="0e717-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e717-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="0e717-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e717-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e717-106">分配给用户的角色定义和角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="0e717-106">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="0e717-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e717-107">Properties</span></span>
|<span data-ttu-id="0e717-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e717-108">Property</span></span>|<span data-ttu-id="0e717-109">类型</span><span class="sxs-lookup"><span data-stu-id="0e717-109">Type</span></span>|<span data-ttu-id="0e717-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e717-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e717-111">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="0e717-111">roleDefinitionIds</span></span>|<span data-ttu-id="0e717-112">String collection</span><span class="sxs-lookup"><span data-stu-id="0e717-112">String collection</span></span>|<span data-ttu-id="0e717-113">分配给用户的表列角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="0e717-113">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="0e717-114">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="0e717-114">roleAssignmentIds</span></span>|<span data-ttu-id="0e717-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0e717-115">String collection</span></span>|<span data-ttu-id="0e717-116">分配给用户的表列角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="0e717-116">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e717-117">关系</span><span class="sxs-lookup"><span data-stu-id="0e717-117">Relationships</span></span>
<span data-ttu-id="0e717-118">无</span><span class="sxs-lookup"><span data-stu-id="0e717-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e717-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e717-119">JSON Representation</span></span>
<span data-ttu-id="0e717-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e717-120">Here is a JSON representation of the resource.</span></span>
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




