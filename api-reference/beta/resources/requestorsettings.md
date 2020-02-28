---
title: requestorSettings 复杂类型
description: 用于访问包`requestorSettings`分配策略的属性。 提供用于选择可以创建请求的何人的其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3205a6ef07c5cf09d8faeb07d19d760872d1e6
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331351"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="0f0c2-104">requestorSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f0c2-104">requestorSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f0c2-105">用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestorSettings**属性。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-105">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0f0c2-106">提供其他设置，以选择可在该策略上为访问包创建请求的成员。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-106">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="0f0c2-107">谁可以请求</span><span class="sxs-lookup"><span data-stu-id="0f0c2-107">Who can request</span></span> | <span data-ttu-id="0f0c2-108">scopeType</span><span class="sxs-lookup"><span data-stu-id="0f0c2-108">scopeType</span></span> | <span data-ttu-id="0f0c2-109">allowedRequestors 集合</span><span class="sxs-lookup"><span data-stu-id="0f0c2-109">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="0f0c2-110">没人</span><span class="sxs-lookup"><span data-stu-id="0f0c2-110">No one</span></span>|`NoSubjects`|<span data-ttu-id="0f0c2-111">空数组</span><span class="sxs-lookup"><span data-stu-id="0f0c2-111">empty array</span></span>|
|<span data-ttu-id="0f0c2-112">目录中的特定个人用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-112">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="0f0c2-113">singleUser</span><span class="sxs-lookup"><span data-stu-id="0f0c2-113">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="0f0c2-114">目录中属于组成员的用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-114">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="0f0c2-115">groupMembers</span><span class="sxs-lookup"><span data-stu-id="0f0c2-115">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="0f0c2-116">目录中`userType`值为的用户`member`</span><span class="sxs-lookup"><span data-stu-id="0f0c2-116">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="0f0c2-117">空数组</span><span class="sxs-lookup"><span data-stu-id="0f0c2-117">empty array</span></span>|
|<span data-ttu-id="0f0c2-118">目录中的用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-118">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="0f0c2-119">空数组</span><span class="sxs-lookup"><span data-stu-id="0f0c2-119">empty array</span></span>|
|<span data-ttu-id="0f0c2-120">已配置特定其他连接组织中的用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-120">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="0f0c2-121">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="0f0c2-121">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="0f0c2-122">已配置的任何其他已连接组织的用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-122">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="0f0c2-123">空数组</span><span class="sxs-lookup"><span data-stu-id="0f0c2-123">empty array</span></span>|
|<span data-ttu-id="0f0c2-124">任何用户</span><span class="sxs-lookup"><span data-stu-id="0f0c2-124">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="0f0c2-125">空数组</span><span class="sxs-lookup"><span data-stu-id="0f0c2-125">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="0f0c2-126">属性</span><span class="sxs-lookup"><span data-stu-id="0f0c2-126">Properties</span></span>

| <span data-ttu-id="0f0c2-127">属性</span><span class="sxs-lookup"><span data-stu-id="0f0c2-127">Property</span></span>                     | <span data-ttu-id="0f0c2-128">类型</span><span class="sxs-lookup"><span data-stu-id="0f0c2-128">Type</span></span>                      | <span data-ttu-id="0f0c2-129">说明</span><span class="sxs-lookup"><span data-stu-id="0f0c2-129">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0f0c2-130">scopeType</span><span class="sxs-lookup"><span data-stu-id="0f0c2-130">scopeType</span></span> |<span data-ttu-id="0f0c2-131">String</span><span class="sxs-lookup"><span data-stu-id="0f0c2-131">String</span></span> |<span data-ttu-id="0f0c2-132">谁可以请求。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-132">Who can request.</span></span> <span data-ttu-id="0f0c2-133">、、 `NoSubjects`、 `SpecificDirectorySubjects`、 `SpecificConnectedOrganizationSubjects` `AllExistingDirectorySubjects`或`AllExistingConnectedOrganizationSubjects` `AllExternalSubjects`中`AllExistingDirectoryMemberUsers`的一个。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-133">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="0f0c2-134">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="0f0c2-134">acceptRequests</span></span> | <span data-ttu-id="0f0c2-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="0f0c2-135">Boolean</span></span> | <span data-ttu-id="0f0c2-136">指示是否在此策略上接受新的请求。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-136">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="0f0c2-137">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="0f0c2-137">allowedRequestors</span></span> | <span data-ttu-id="0f0c2-138">[userSet](userset.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f0c2-138">[userSet](userset.md) collection</span></span>| <span data-ttu-id="0f0c2-139">允许对此策略提出请求的用户，可以是[singleUser](singleuser.md)、 [groupMembers](groupmembers.md)和[connectedOrganizationMembers](connectedorganizationmembers.md)。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-139">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f0c2-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f0c2-140">JSON representation</span></span>


<span data-ttu-id="0f0c2-141">以下是策略的**requestorSettings**属性的 JSON 表示形式，它允许组的成员请求。</span><span class="sxs-lookup"><span data-stu-id="0f0c2-141">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
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
