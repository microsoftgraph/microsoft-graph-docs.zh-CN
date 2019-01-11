---
title: governancePermission 资源类型
description: '表示对特定 governanceResource governanceSubject 具有访问权限。  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882871"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="73f66-103">governancePermission 资源类型</span><span class="sxs-lookup"><span data-stu-id="73f66-103">governancePermission resource type</span></span>

> <span data-ttu-id="73f66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73f66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73f66-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73f66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73f66-106">表示对特定[governanceResource](../resources/governanceresource.md) [governanceSubject](../resources/governancesubject.md)具有访问权限。</span><span class="sxs-lookup"><span data-stu-id="73f66-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="73f66-107">属性</span><span class="sxs-lookup"><span data-stu-id="73f66-107">Properties</span></span>
| <span data-ttu-id="73f66-108">属性</span><span class="sxs-lookup"><span data-stu-id="73f66-108">Property</span></span>     | <span data-ttu-id="73f66-109">类型</span><span class="sxs-lookup"><span data-stu-id="73f66-109">Type</span></span>   |<span data-ttu-id="73f66-110">Description</span><span class="sxs-lookup"><span data-stu-id="73f66-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73f66-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="73f66-111">accessLevel</span></span>|<span data-ttu-id="73f66-112">字符串</span><span class="sxs-lookup"><span data-stu-id="73f66-112">String</span></span>|<span data-ttu-id="73f66-113">访问级别。</span><span class="sxs-lookup"><span data-stu-id="73f66-113">The access level.</span></span> <span data-ttu-id="73f66-114">有效值： ``None``， ``UserRead``， ``AdminRead``，和``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="73f66-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="73f66-115">isActive</span><span class="sxs-lookup"><span data-stu-id="73f66-115">isActive</span></span>|<span data-ttu-id="73f66-116">布尔</span><span class="sxs-lookup"><span data-stu-id="73f66-116">Boolean</span></span>|<span data-ttu-id="73f66-117">指示如果请求者有任何主动角色分配访问级别。</span><span class="sxs-lookup"><span data-stu-id="73f66-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="73f66-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="73f66-118">isEligible</span></span>|<span data-ttu-id="73f66-119">布尔</span><span class="sxs-lookup"><span data-stu-id="73f66-119">Boolean</span></span>|<span data-ttu-id="73f66-120">指示请求者是否具有任何访问级别的合格的角色分配。</span><span class="sxs-lookup"><span data-stu-id="73f66-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73f66-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73f66-121">JSON representation</span></span>

<span data-ttu-id="73f66-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73f66-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
