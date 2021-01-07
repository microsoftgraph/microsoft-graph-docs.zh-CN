---
title: requestorSettings 复杂类型
description: 用于 `requestorSettings` 访问包分配策略的属性。 提供其他设置，以选择可以创建请求的人。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccaa57a3dfa2f81d33e4e6fea804a91d1db7da20
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777608"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="24bef-104">requestorSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="24bef-104">requestorSettings resource type</span></span>

<span data-ttu-id="24bef-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24bef-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24bef-106">用于访问 **包分配策略的 requestorSettings** [属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="24bef-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="24bef-107">提供其他设置，以选择可以在该策略上创建访问包请求的人。</span><span class="sxs-lookup"><span data-stu-id="24bef-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="24bef-108">谁可以请求</span><span class="sxs-lookup"><span data-stu-id="24bef-108">Who can request</span></span> | <span data-ttu-id="24bef-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="24bef-109">scopeType</span></span> | <span data-ttu-id="24bef-110">allowedRequestors 集合</span><span class="sxs-lookup"><span data-stu-id="24bef-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="24bef-111">没人</span><span class="sxs-lookup"><span data-stu-id="24bef-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="24bef-112">空数组</span><span class="sxs-lookup"><span data-stu-id="24bef-112">empty array</span></span>|
|<span data-ttu-id="24bef-113">目录中的特定单个用户</span><span class="sxs-lookup"><span data-stu-id="24bef-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="24bef-114">singleUser</span><span class="sxs-lookup"><span data-stu-id="24bef-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="24bef-115">目录中作为组成员的用户</span><span class="sxs-lookup"><span data-stu-id="24bef-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="24bef-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="24bef-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="24bef-117">目录中值为 `userType``member`</span><span class="sxs-lookup"><span data-stu-id="24bef-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="24bef-118">空数组</span><span class="sxs-lookup"><span data-stu-id="24bef-118">empty array</span></span>|
|<span data-ttu-id="24bef-119">目录中的用户</span><span class="sxs-lookup"><span data-stu-id="24bef-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="24bef-120">空数组</span><span class="sxs-lookup"><span data-stu-id="24bef-120">empty array</span></span>|
|<span data-ttu-id="24bef-121">特定连接组织中用户</span><span class="sxs-lookup"><span data-stu-id="24bef-121">Users in specific connected organizations</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="24bef-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="24bef-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="24bef-123">已连接组织的状态属性设置为的任何已连接组织的用户 `configured` 。</span><span class="sxs-lookup"><span data-stu-id="24bef-123">Users from any connected organizations that have the state property of the connected organization set to `configured`.</span></span>|`AllConfiguredConnectedOrganizationSubjects`|<span data-ttu-id="24bef-124">空数组</span><span class="sxs-lookup"><span data-stu-id="24bef-124">empty array</span></span>|
|<span data-ttu-id="24bef-125">任何用户</span><span class="sxs-lookup"><span data-stu-id="24bef-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="24bef-126">空数组</span><span class="sxs-lookup"><span data-stu-id="24bef-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="24bef-127">属性</span><span class="sxs-lookup"><span data-stu-id="24bef-127">Properties</span></span>

| <span data-ttu-id="24bef-128">属性</span><span class="sxs-lookup"><span data-stu-id="24bef-128">Property</span></span>                     | <span data-ttu-id="24bef-129">类型</span><span class="sxs-lookup"><span data-stu-id="24bef-129">Type</span></span>                      | <span data-ttu-id="24bef-130">说明</span><span class="sxs-lookup"><span data-stu-id="24bef-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="24bef-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="24bef-131">scopeType</span></span> |<span data-ttu-id="24bef-132">String</span><span class="sxs-lookup"><span data-stu-id="24bef-132">String</span></span> |<span data-ttu-id="24bef-133">谁可以请求。</span><span class="sxs-lookup"><span data-stu-id="24bef-133">Who can request.</span></span> <span data-ttu-id="24bef-134">、 `NoSubjects` `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` 或 `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` 。</span><span class="sxs-lookup"><span data-stu-id="24bef-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllConfiguredConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="24bef-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="24bef-135">acceptRequests</span></span> | <span data-ttu-id="24bef-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="24bef-136">Boolean</span></span> | <span data-ttu-id="24bef-137">指示此策略是否接受新请求。</span><span class="sxs-lookup"><span data-stu-id="24bef-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="24bef-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="24bef-138">allowedRequestors</span></span> | <span data-ttu-id="24bef-139">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24bef-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="24bef-140">允许在此策略上请求的用户，可以是[singleUser、groupMembers](groupmembers.md)和[connectedOrganizationMembers。](connectedorganizationmembers.md) [](singleuser.md)</span><span class="sxs-lookup"><span data-stu-id="24bef-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24bef-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24bef-141">JSON representation</span></span>


<span data-ttu-id="24bef-142">下面是策略 **的 requestorSettings** 属性的 JSON 表示形式，允许组的成员进行请求。</span><span class="sxs-lookup"><span data-stu-id="24bef-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


