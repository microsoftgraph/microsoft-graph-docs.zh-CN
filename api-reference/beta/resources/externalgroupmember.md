---
title: externalGroupMember 资源类型
description: 表示用于设置对添加到 Microsoft Graph 的外部内容的权限的外部组的成员。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161689"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="f97ea-103">externalGroupMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="f97ea-103">externalGroupMember resource type</span></span>

<span data-ttu-id="f97ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f97ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f97ea-105">表示用于设置 [对](externalgroup.md) 添加到 Microsoft Graph 的外部内容的权限的外部组的成员。</span><span class="sxs-lookup"><span data-stu-id="f97ea-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="f97ea-106">方法</span><span class="sxs-lookup"><span data-stu-id="f97ea-106">Methods</span></span>

| <span data-ttu-id="f97ea-107">方法</span><span class="sxs-lookup"><span data-stu-id="f97ea-107">Method</span></span>                                                              | <span data-ttu-id="f97ea-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f97ea-108">Return type</span></span>         | <span data-ttu-id="f97ea-109">说明</span><span class="sxs-lookup"><span data-stu-id="f97ea-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="f97ea-110">创建 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f97ea-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="f97ea-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f97ea-111">externalGroupMember</span></span> | <span data-ttu-id="f97ea-112">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="f97ea-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="f97ea-113">删除 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f97ea-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="f97ea-114">无</span><span class="sxs-lookup"><span data-stu-id="f97ea-114">None</span></span>                | <span data-ttu-id="f97ea-115">删除 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="f97ea-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="f97ea-116">属性</span><span class="sxs-lookup"><span data-stu-id="f97ea-116">Properties</span></span>

| <span data-ttu-id="f97ea-117">属性</span><span class="sxs-lookup"><span data-stu-id="f97ea-117">Property</span></span>       | <span data-ttu-id="f97ea-118">类型</span><span class="sxs-lookup"><span data-stu-id="f97ea-118">Type</span></span>                    | <span data-ttu-id="f97ea-119">说明</span><span class="sxs-lookup"><span data-stu-id="f97ea-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="f97ea-120">id</span><span class="sxs-lookup"><span data-stu-id="f97ea-120">id</span></span>             | <span data-ttu-id="f97ea-121">String</span><span class="sxs-lookup"><span data-stu-id="f97ea-121">String</span></span>                  | <span data-ttu-id="f97ea-122">成员的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f97ea-122">The unique ID of the member.</span></span> <span data-ttu-id="f97ea-123">对于 Azure Active Directory 用户或组，它将是 objectId，对于外部组，为 **externalGroup** 的 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="f97ea-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="f97ea-124">type</span><span class="sxs-lookup"><span data-stu-id="f97ea-124">type</span></span>           | <span data-ttu-id="f97ea-125">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="f97ea-125">externalGroupMemberType</span></span> | <span data-ttu-id="f97ea-126">添加到外部组的成员的类型。</span><span class="sxs-lookup"><span data-stu-id="f97ea-126">The type of member added to the external group.</span></span> <span data-ttu-id="f97ea-127">可能的值是： `user` 或 `group` 当 **identitySource** 是时，或者 `azureActiveDirectory` 当 `group` **identitySource** 为时 `external` 。</span><span class="sxs-lookup"><span data-stu-id="f97ea-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="f97ea-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="f97ea-128">identitySource</span></span> | <span data-ttu-id="f97ea-129">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="f97ea-129">identitySourceType</span></span>      | <span data-ttu-id="f97ea-130">成员所属的标识源。</span><span class="sxs-lookup"><span data-stu-id="f97ea-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="f97ea-131">可取值为：`azureActiveDirectory`、`external`。</span><span class="sxs-lookup"><span data-stu-id="f97ea-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="f97ea-132">关系</span><span class="sxs-lookup"><span data-stu-id="f97ea-132">Relationships</span></span>

<span data-ttu-id="f97ea-133">无。</span><span class="sxs-lookup"><span data-stu-id="f97ea-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f97ea-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f97ea-134">JSON representation</span></span>

<span data-ttu-id="f97ea-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f97ea-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
