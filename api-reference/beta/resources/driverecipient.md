---
author: JeremyKelley
description: DriveRecipient 资源表示用户、组或其他收件人使用 invite 操作进行共享。
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f703aa1bc9d12ec8b67aab0d80d641964b7b6096
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058471"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="24f59-103">DriveRecipient 资源</span><span class="sxs-lookup"><span data-stu-id="24f59-103">DriveRecipient resource</span></span>

<span data-ttu-id="24f59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24f59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24f59-105">**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。</span><span class="sxs-lookup"><span data-stu-id="24f59-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24f59-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24f59-106">JSON representation</span></span>

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

## <a name="properties"></a><span data-ttu-id="24f59-107">属性</span><span class="sxs-lookup"><span data-stu-id="24f59-107">Properties</span></span>
<span data-ttu-id="24f59-108">收件人资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="24f59-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="24f59-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="24f59-109">Property name</span></span> | <span data-ttu-id="24f59-110">类型</span><span class="sxs-lookup"><span data-stu-id="24f59-110">Type</span></span>   | <span data-ttu-id="24f59-111">说明</span><span class="sxs-lookup"><span data-stu-id="24f59-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="24f59-112">email</span><span class="sxs-lookup"><span data-stu-id="24f59-112">email</span></span>         | <span data-ttu-id="24f59-113">String</span><span class="sxs-lookup"><span data-stu-id="24f59-113">String</span></span> | <span data-ttu-id="24f59-114">收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="24f59-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="24f59-115">别名</span><span class="sxs-lookup"><span data-stu-id="24f59-115">alias</span></span>         | <span data-ttu-id="24f59-116">String</span><span class="sxs-lookup"><span data-stu-id="24f59-116">String</span></span> | <span data-ttu-id="24f59-117">Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。</span><span class="sxs-lookup"><span data-stu-id="24f59-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="24f59-118">objectId</span><span class="sxs-lookup"><span data-stu-id="24f59-118">objectId</span></span>      | <span data-ttu-id="24f59-119">String</span><span class="sxs-lookup"><span data-stu-id="24f59-119">String</span></span> | <span data-ttu-id="24f59-120">目录中收件人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="24f59-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="24f59-121">注解</span><span class="sxs-lookup"><span data-stu-id="24f59-121">Remarks</span></span>

<span data-ttu-id="24f59-p101">当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。</span><span class="sxs-lookup"><span data-stu-id="24f59-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->


