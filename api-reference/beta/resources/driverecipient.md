---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ecf3e600cc943d0c82da38928d8018e6c654fb4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525799"
---
# <a name="driverecipient-resource"></a><span data-ttu-id="4b519-102">DriveRecipient 资源</span><span class="sxs-lookup"><span data-stu-id="4b519-102">DriveRecipient resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b519-103">**DriveRecipient** 资源表示用户、组或其他收件人使用 [invite](../api/driveitem-invite.md) 操作进行共享。</span><span class="sxs-lookup"><span data-stu-id="4b519-103">The **DriveRecipient** resource represents a person, group, or other recipient to share with using the [invite](../api/driveitem-invite.md) action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b519-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b519-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4b519-105">属性</span><span class="sxs-lookup"><span data-stu-id="4b519-105">Properties</span></span>
<span data-ttu-id="4b519-106">收件人资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="4b519-106">The recipients resource has these properties.</span></span>

| <span data-ttu-id="4b519-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="4b519-107">Property name</span></span> | <span data-ttu-id="4b519-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b519-108">Type</span></span>   | <span data-ttu-id="4b519-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b519-109">Description</span></span>                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b519-110">email</span><span class="sxs-lookup"><span data-stu-id="4b519-110">email</span></span>         | <span data-ttu-id="4b519-111">String</span><span class="sxs-lookup"><span data-stu-id="4b519-111">String</span></span> | <span data-ttu-id="4b519-112">收件人的电子邮件地址，前提是收件人有关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4b519-112">The email address for the recipient, if the recipient has an associated email address.</span></span>                  |
| <span data-ttu-id="4b519-113">别名</span><span class="sxs-lookup"><span data-stu-id="4b519-113">alias</span></span>         | <span data-ttu-id="4b519-114">String</span><span class="sxs-lookup"><span data-stu-id="4b519-114">String</span></span> | <span data-ttu-id="4b519-115">Domain 对象的别名，适于电子邮件地址不可用的情况（例如，安全组）。</span><span class="sxs-lookup"><span data-stu-id="4b519-115">The alias of the domain object, for cases where an email address is unavailable (e.g. security groups).</span></span> |
| <span data-ttu-id="4b519-116">objectId</span><span class="sxs-lookup"><span data-stu-id="4b519-116">objectId</span></span>      | <span data-ttu-id="4b519-117">String</span><span class="sxs-lookup"><span data-stu-id="4b519-117">String</span></span> | <span data-ttu-id="4b519-118">目录中收件人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4b519-118">The unique identifier for the recipient in the directory.</span></span>                                               |

## <a name="remarks"></a><span data-ttu-id="4b519-119">注解</span><span class="sxs-lookup"><span data-stu-id="4b519-119">Remarks</span></span>

<span data-ttu-id="4b519-p101">当使用 [邀请](../api/driveitem-invite.md) 添加权限时，DriveRecipient 可以指定**电子邮件**、**别名**或**对象 ID**。这些值中只有一个是必需的。</span><span class="sxs-lookup"><span data-stu-id="4b519-p101">When using [invite](../api/driveitem-invite.md) to add permissions, the DriveRecipient can specify **email**, **alias**, or **objectId**. Only one of these values is required.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": [
    "Error: /api-reference/beta/resources/driverecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
