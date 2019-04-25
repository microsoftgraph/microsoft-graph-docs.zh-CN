---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 47a080b4f81645cfe5098ec8391d58cf07fca466
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543145"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="d2551-102">DriveRecipient 资源</span><span class="sxs-lookup"><span data-stu-id="d2551-102">DriveRecipient resource</span></span>

<span data-ttu-id="d2551-103">**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。</span><span class="sxs-lookup"><span data-stu-id="d2551-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2551-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2551-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d2551-105">属性</span><span class="sxs-lookup"><span data-stu-id="d2551-105">Properties</span></span>
<span data-ttu-id="d2551-106">收件人资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="d2551-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="d2551-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="d2551-107">Property name</span></span> | <span data-ttu-id="d2551-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2551-108">Type</span></span>   | <span data-ttu-id="d2551-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2551-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d2551-110">email</span><span class="sxs-lookup"><span data-stu-id="d2551-110">email</span></span>         | <span data-ttu-id="d2551-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d2551-111">String</span></span> | <span data-ttu-id="d2551-112">收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d2551-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="d2551-113">别名</span><span class="sxs-lookup"><span data-stu-id="d2551-113">alias</span></span>         | <span data-ttu-id="d2551-114">String</span><span class="sxs-lookup"><span data-stu-id="d2551-114">String</span></span> | <span data-ttu-id="d2551-115">Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。</span><span class="sxs-lookup"><span data-stu-id="d2551-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="d2551-116">objectId</span><span class="sxs-lookup"><span data-stu-id="d2551-116">objectId</span></span>      | <span data-ttu-id="d2551-117">String</span><span class="sxs-lookup"><span data-stu-id="d2551-117">String</span></span> | <span data-ttu-id="d2551-118">目录中收件人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2551-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="d2551-119">注解</span><span class="sxs-lookup"><span data-stu-id="d2551-119">Remarks</span></span>

<span data-ttu-id="d2551-p101">当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。</span><span class="sxs-lookup"><span data-stu-id="d2551-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
