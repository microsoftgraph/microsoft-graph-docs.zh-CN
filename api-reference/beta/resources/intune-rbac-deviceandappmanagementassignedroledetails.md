---
title: deviceAndAppManagementAssignedRoleDetails 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d6ace16ba496feb24948c3e40c32dd8fcb2fcf48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428852"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="e2920-103">deviceAndAppManagementAssignedRoleDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2920-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="e2920-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e2920-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2920-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2920-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2920-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e2920-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e2920-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2920-108">Properties</span></span>
|<span data-ttu-id="e2920-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2920-109">Property</span></span>|<span data-ttu-id="e2920-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2920-110">Type</span></span>|<span data-ttu-id="e2920-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2920-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2920-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="e2920-112">roleDefinitionIds</span></span>|<span data-ttu-id="e2920-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="e2920-113">String collection</span></span>|<span data-ttu-id="e2920-114">特定分配给用户的角色定义的角色定义 Id。</span><span class="sxs-lookup"><span data-stu-id="e2920-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="e2920-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="e2920-115">roleAssignmentIds</span></span>|<span data-ttu-id="e2920-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="e2920-116">String collection</span></span>|<span data-ttu-id="e2920-117">特定分配给用户的角色分配的角色分配 Id。</span><span class="sxs-lookup"><span data-stu-id="e2920-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2920-118">关系</span><span class="sxs-lookup"><span data-stu-id="e2920-118">Relationships</span></span>
<span data-ttu-id="e2920-119">无</span><span class="sxs-lookup"><span data-stu-id="e2920-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2920-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2920-120">JSON Representation</span></span>
<span data-ttu-id="e2920-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2920-121">Here is a JSON representation of the resource.</span></span>
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




