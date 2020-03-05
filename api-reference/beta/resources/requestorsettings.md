---
title: requestorSettings 复杂类型
description: 用于访问包`requestorSettings`分配策略的属性。 提供用于选择可以创建请求的何人的其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b52f3276185f819ccd0e7149dbd5420b4f6e1781
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521115"
---
# <a name="requestorsettings-resource-type"></a><span data-ttu-id="1b07b-104">requestorSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b07b-104">requestorSettings resource type</span></span>

<span data-ttu-id="1b07b-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b07b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b07b-106">用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestorSettings**属性。</span><span class="sxs-lookup"><span data-stu-id="1b07b-106">Used for the **requestorSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="1b07b-107">提供其他设置，以选择可在该策略上为访问包创建请求的成员。</span><span class="sxs-lookup"><span data-stu-id="1b07b-107">Provides additional settings to select who can create a request for an access package on that policy.</span></span>

| <span data-ttu-id="1b07b-108">谁可以请求</span><span class="sxs-lookup"><span data-stu-id="1b07b-108">Who can request</span></span> | <span data-ttu-id="1b07b-109">scopeType</span><span class="sxs-lookup"><span data-stu-id="1b07b-109">scopeType</span></span> | <span data-ttu-id="1b07b-110">allowedRequestors 集合</span><span class="sxs-lookup"><span data-stu-id="1b07b-110">allowedRequestors collection</span></span>|
|:----------------|:----------|:------------------|
|<span data-ttu-id="1b07b-111">没人</span><span class="sxs-lookup"><span data-stu-id="1b07b-111">No one</span></span>|`NoSubjects`|<span data-ttu-id="1b07b-112">空数组</span><span class="sxs-lookup"><span data-stu-id="1b07b-112">empty array</span></span>|
|<span data-ttu-id="1b07b-113">目录中的特定个人用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-113">Specific individual user in your directory</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="1b07b-114">singleUser</span><span class="sxs-lookup"><span data-stu-id="1b07b-114">singleUser</span></span>](singleuser.md)|
|<span data-ttu-id="1b07b-115">目录中属于组成员的用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-115">Users in your directory who are members of a group</span></span>|`SpecificDirectorySubjects`|[<span data-ttu-id="1b07b-116">groupMembers</span><span class="sxs-lookup"><span data-stu-id="1b07b-116">groupMembers</span></span>](groupmembers.md)|
|<span data-ttu-id="1b07b-117">目录中`userType`值为的用户`member`</span><span class="sxs-lookup"><span data-stu-id="1b07b-117">Users in your directory with `userType` value of `member`</span></span>|`AllExistingDirectoryMemberUsers`|<span data-ttu-id="1b07b-118">空数组</span><span class="sxs-lookup"><span data-stu-id="1b07b-118">empty array</span></span>|
|<span data-ttu-id="1b07b-119">目录中的用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-119">Users in your directory</span></span>|`AllExistingDirectorySubjects`|<span data-ttu-id="1b07b-120">空数组</span><span class="sxs-lookup"><span data-stu-id="1b07b-120">empty array</span></span>|
|<span data-ttu-id="1b07b-121">已配置特定其他连接组织中的用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-121">Users in specific other connected organizations already configured</span></span>|`SpecificConnectedOrganizationSubjects`|[<span data-ttu-id="1b07b-122">connectedOrganizationMembers</span><span class="sxs-lookup"><span data-stu-id="1b07b-122">connectedOrganizationMembers</span></span>](connectedorganizationmembers.md)|
|<span data-ttu-id="1b07b-123">已配置的任何其他已连接组织的用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-123">Users from any other connected organizations already configured</span></span>|`AllExistingConnectedOrganizationSubjects`|<span data-ttu-id="1b07b-124">空数组</span><span class="sxs-lookup"><span data-stu-id="1b07b-124">empty array</span></span>|
|<span data-ttu-id="1b07b-125">任何用户</span><span class="sxs-lookup"><span data-stu-id="1b07b-125">Any user</span></span>|`AllExternalSubjects`|<span data-ttu-id="1b07b-126">空数组</span><span class="sxs-lookup"><span data-stu-id="1b07b-126">empty array</span></span>|

## <a name="properties"></a><span data-ttu-id="1b07b-127">属性</span><span class="sxs-lookup"><span data-stu-id="1b07b-127">Properties</span></span>

| <span data-ttu-id="1b07b-128">属性</span><span class="sxs-lookup"><span data-stu-id="1b07b-128">Property</span></span>                     | <span data-ttu-id="1b07b-129">类型</span><span class="sxs-lookup"><span data-stu-id="1b07b-129">Type</span></span>                      | <span data-ttu-id="1b07b-130">说明</span><span class="sxs-lookup"><span data-stu-id="1b07b-130">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="1b07b-131">scopeType</span><span class="sxs-lookup"><span data-stu-id="1b07b-131">scopeType</span></span> |<span data-ttu-id="1b07b-132">String</span><span class="sxs-lookup"><span data-stu-id="1b07b-132">String</span></span> |<span data-ttu-id="1b07b-133">谁可以请求。</span><span class="sxs-lookup"><span data-stu-id="1b07b-133">Who can request.</span></span> <span data-ttu-id="1b07b-134">、、 `NoSubjects`、 `SpecificDirectorySubjects`、 `SpecificConnectedOrganizationSubjects` `AllExistingDirectorySubjects`或`AllExistingConnectedOrganizationSubjects` `AllExternalSubjects`中`AllExistingDirectoryMemberUsers`的一个。</span><span class="sxs-lookup"><span data-stu-id="1b07b-134">One of `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers`, `AllExistingDirectorySubjects` or `AllExternalSubjects`.</span></span>  |
| <span data-ttu-id="1b07b-135">acceptRequests</span><span class="sxs-lookup"><span data-stu-id="1b07b-135">acceptRequests</span></span> | <span data-ttu-id="1b07b-136">布尔</span><span class="sxs-lookup"><span data-stu-id="1b07b-136">Boolean</span></span> | <span data-ttu-id="1b07b-137">指示是否在此策略上接受新的请求。</span><span class="sxs-lookup"><span data-stu-id="1b07b-137">Indicates whether new requests are accepted on this policy.</span></span> |
| <span data-ttu-id="1b07b-138">allowedRequestors</span><span class="sxs-lookup"><span data-stu-id="1b07b-138">allowedRequestors</span></span> | <span data-ttu-id="1b07b-139">[userSet](userset.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b07b-139">[userSet](userset.md) collection</span></span>| <span data-ttu-id="1b07b-140">允许对此策略提出请求的用户，可以是[singleUser](singleuser.md)、 [groupMembers](groupmembers.md)和[connectedOrganizationMembers](connectedorganizationmembers.md)。</span><span class="sxs-lookup"><span data-stu-id="1b07b-140">The users who are allowed to request on this policy, which can be [singleUser](singleuser.md), [groupMembers](groupmembers.md), and [connectedOrganizationMembers](connectedorganizationmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b07b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b07b-141">JSON representation</span></span>


<span data-ttu-id="1b07b-142">以下是策略的**requestorSettings**属性的 JSON 表示形式，它允许组的成员请求。</span><span class="sxs-lookup"><span data-stu-id="1b07b-142">The following is a JSON representation of the **requestorSettings** property of a policy, which allows the members of a group to request.</span></span>

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
