---
title: educationIdentityDomain 资源类型
description: '表示教育用户类型与用户帐户所属域之间的映射。 域资源是标识创建配置的一部分。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543075"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="2838f-104">educationIdentityDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="2838f-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2838f-105">表示教育用户类型与用户帐户所属域之间的映射。</span><span class="sxs-lookup"><span data-stu-id="2838f-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="2838f-106">域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="2838f-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="2838f-107">属性</span><span class="sxs-lookup"><span data-stu-id="2838f-107">Properties</span></span>

| <span data-ttu-id="2838f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2838f-108">Property</span></span> | <span data-ttu-id="2838f-109">类型</span><span class="sxs-lookup"><span data-stu-id="2838f-109">Type</span></span> | <span data-ttu-id="2838f-110">说明</span><span class="sxs-lookup"><span data-stu-id="2838f-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2838f-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="2838f-111">**appliesTo**</span></span> | <span data-ttu-id="2838f-112">string</span><span class="sxs-lookup"><span data-stu-id="2838f-112">string</span></span> |  <span data-ttu-id="2838f-113">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="2838f-113">The user role type to assign to license.</span></span> <span data-ttu-id="2838f-114">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="2838f-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="2838f-115">**name**</span><span class="sxs-lookup"><span data-stu-id="2838f-115">**name**</span></span> | <span data-ttu-id="2838f-116">string</span><span class="sxs-lookup"><span data-stu-id="2838f-116">string</span></span> |  <span data-ttu-id="2838f-117">代表用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="2838f-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="2838f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2838f-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
