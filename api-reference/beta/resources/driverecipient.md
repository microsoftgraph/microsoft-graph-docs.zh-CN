---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.openlocfilehash: f1bc78a8ec0648ce90221e4ad1f4473e49b625b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863726"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="1a56f-102">DriveRecipient 资源</span><span class="sxs-lookup"><span data-stu-id="1a56f-102">DriveRecipient resource</span></span>

> <span data-ttu-id="1a56f-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a56f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a56f-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a56f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1a56f-105">**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。</span><span class="sxs-lookup"><span data-stu-id="1a56f-105">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a56f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a56f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1a56f-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a56f-107">Properties</span></span>
<span data-ttu-id="1a56f-108">收件人资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="1a56f-108">The recipients resource has these properties.</span></span>

| <span data-ttu-id="1a56f-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="1a56f-109">Property name</span></span> | <span data-ttu-id="1a56f-110">类型</span><span class="sxs-lookup"><span data-stu-id="1a56f-110">Type</span></span>   | <span data-ttu-id="1a56f-111">说明</span><span class="sxs-lookup"><span data-stu-id="1a56f-111">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1a56f-112">email</span><span class="sxs-lookup"><span data-stu-id="1a56f-112">email</span></span>         | <span data-ttu-id="1a56f-113">String</span><span class="sxs-lookup"><span data-stu-id="1a56f-113">String</span></span> | <span data-ttu-id="1a56f-114">收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1a56f-114">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="1a56f-115">别名</span><span class="sxs-lookup"><span data-stu-id="1a56f-115">alias</span></span>         | <span data-ttu-id="1a56f-116">String</span><span class="sxs-lookup"><span data-stu-id="1a56f-116">String</span></span> | <span data-ttu-id="1a56f-117">Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。</span><span class="sxs-lookup"><span data-stu-id="1a56f-117">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="1a56f-118">objectId</span><span class="sxs-lookup"><span data-stu-id="1a56f-118">objectId</span></span>      | <span data-ttu-id="1a56f-119">String</span><span class="sxs-lookup"><span data-stu-id="1a56f-119">String</span></span> | <span data-ttu-id="1a56f-120">目录中收件人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1a56f-120">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="1a56f-121">注解</span><span class="sxs-lookup"><span data-stu-id="1a56f-121">Remarks</span></span>

<span data-ttu-id="1a56f-p102">当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。</span><span class="sxs-lookup"><span data-stu-id="1a56f-p102">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
