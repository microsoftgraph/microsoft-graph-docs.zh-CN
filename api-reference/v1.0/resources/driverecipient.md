---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4792a943598911cc2f0b8329016469ca157bda58
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480325"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="70ee0-102">DriveRecipient 资源</span><span class="sxs-lookup"><span data-stu-id="70ee0-102">DriveRecipient resource</span></span>

<span data-ttu-id="70ee0-103">**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。</span><span class="sxs-lookup"><span data-stu-id="70ee0-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70ee0-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70ee0-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="70ee0-105">属性</span><span class="sxs-lookup"><span data-stu-id="70ee0-105">Properties</span></span>
<span data-ttu-id="70ee0-106">收件人资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="70ee0-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="70ee0-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="70ee0-107">Property name</span></span> | <span data-ttu-id="70ee0-108">类型</span><span class="sxs-lookup"><span data-stu-id="70ee0-108">Type</span></span>   | <span data-ttu-id="70ee0-109">说明</span><span class="sxs-lookup"><span data-stu-id="70ee0-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="70ee0-110">email</span><span class="sxs-lookup"><span data-stu-id="70ee0-110">email</span></span>         | <span data-ttu-id="70ee0-111">字符串</span><span class="sxs-lookup"><span data-stu-id="70ee0-111">String</span></span> | <span data-ttu-id="70ee0-112">收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="70ee0-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="70ee0-113">别名</span><span class="sxs-lookup"><span data-stu-id="70ee0-113">alias</span></span>         | <span data-ttu-id="70ee0-114">String</span><span class="sxs-lookup"><span data-stu-id="70ee0-114">String</span></span> | <span data-ttu-id="70ee0-115">Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。</span><span class="sxs-lookup"><span data-stu-id="70ee0-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="70ee0-116">objectId</span><span class="sxs-lookup"><span data-stu-id="70ee0-116">objectId</span></span>      | <span data-ttu-id="70ee0-117">String</span><span class="sxs-lookup"><span data-stu-id="70ee0-117">String</span></span> | <span data-ttu-id="70ee0-118">目录中收件人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70ee0-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="70ee0-119">注解</span><span class="sxs-lookup"><span data-stu-id="70ee0-119">Remarks</span></span>

<span data-ttu-id="70ee0-p101">当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。</span><span class="sxs-lookup"><span data-stu-id="70ee0-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->
