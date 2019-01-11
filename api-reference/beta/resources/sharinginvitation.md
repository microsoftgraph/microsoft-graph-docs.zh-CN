---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 3ba92573aaef89b1be431ade33caa6ed465917a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835971"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="b80c0-102">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b80c0-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="b80c0-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b80c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b80c0-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b80c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b80c0-105">**SharingInvitation** 资源将与邀请相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="b80c0-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b80c0-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b80c0-106">JSON representation</span></span>

<span data-ttu-id="b80c0-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b80c0-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}

```

## <a name="properties"></a><span data-ttu-id="b80c0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b80c0-108">Properties</span></span>

| <span data-ttu-id="b80c0-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="b80c0-109">Property Name</span></span>  | <span data-ttu-id="b80c0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b80c0-110">Type</span></span>                          | <span data-ttu-id="b80c0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b80c0-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b80c0-112">email</span><span class="sxs-lookup"><span data-stu-id="b80c0-112">email</span></span>          | <span data-ttu-id="b80c0-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b80c0-113">String</span></span>                        | <span data-ttu-id="b80c0-p102">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="b80c0-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="b80c0-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="b80c0-116">invitedBy</span></span>      | [<span data-ttu-id="b80c0-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="b80c0-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="b80c0-p103">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="b80c0-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="b80c0-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="b80c0-120">signInRequired</span></span> | <span data-ttu-id="b80c0-121">布尔</span><span class="sxs-lookup"><span data-stu-id="b80c0-121">Boolean</span></span>                       | <span data-ttu-id="b80c0-p104">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="b80c0-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="b80c0-124">注解</span><span class="sxs-lookup"><span data-stu-id="b80c0-124">Remarks</span></span> 

<span data-ttu-id="b80c0-125">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b80c0-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
