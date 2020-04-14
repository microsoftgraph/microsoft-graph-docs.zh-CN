---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 分配给用户的角色定义和角色分配的集合。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 061929eadd3b636ab8fcc4d89a45489bacfa9aae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467694"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="70726-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="70726-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

<span data-ttu-id="70726-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70726-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70726-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="70726-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70726-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70726-107">分配给用户的角色定义和角色分配的集合。</span><span class="sxs-lookup"><span data-stu-id="70726-107">The set of Role Definitions and Role Assignments assigned to a user.</span></span>

## <a name="properties"></a><span data-ttu-id="70726-108">属性</span><span class="sxs-lookup"><span data-stu-id="70726-108">Properties</span></span>
|<span data-ttu-id="70726-109">属性</span><span class="sxs-lookup"><span data-stu-id="70726-109">Property</span></span>|<span data-ttu-id="70726-110">类型</span><span class="sxs-lookup"><span data-stu-id="70726-110">Type</span></span>|<span data-ttu-id="70726-111">说明</span><span class="sxs-lookup"><span data-stu-id="70726-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70726-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="70726-112">roleDefinitionIds</span></span>|<span data-ttu-id="70726-113">String collection</span><span class="sxs-lookup"><span data-stu-id="70726-113">String collection</span></span>|<span data-ttu-id="70726-114">分配给用户的表列角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="70726-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="70726-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="70726-115">roleAssignmentIds</span></span>|<span data-ttu-id="70726-116">String collection</span><span class="sxs-lookup"><span data-stu-id="70726-116">String collection</span></span>|<span data-ttu-id="70726-117">分配给用户的表列角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="70726-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70726-118">关系</span><span class="sxs-lookup"><span data-stu-id="70726-118">Relationships</span></span>
<span data-ttu-id="70726-119">无</span><span class="sxs-lookup"><span data-stu-id="70726-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70726-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70726-120">JSON Representation</span></span>
<span data-ttu-id="70726-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70726-121">Here is a JSON representation of the resource.</span></span>
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



