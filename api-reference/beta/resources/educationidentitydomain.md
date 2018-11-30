---
title: educationIdentityDomain 资源类型
description: '代表教育用户类型和用户的帐户所属的域之间的映射。 域资源是标识创建配置的一部分。 '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046681"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="bb15a-104">educationIdentityDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb15a-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="bb15a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bb15a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb15a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb15a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb15a-107">代表教育用户类型和用户的帐户所属的域之间的映射。</span><span class="sxs-lookup"><span data-stu-id="bb15a-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="bb15a-108">域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="bb15a-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="bb15a-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb15a-109">Properties</span></span>

| <span data-ttu-id="bb15a-110">属性</span><span class="sxs-lookup"><span data-stu-id="bb15a-110">Property</span></span> | <span data-ttu-id="bb15a-111">类型</span><span class="sxs-lookup"><span data-stu-id="bb15a-111">Type</span></span> | <span data-ttu-id="bb15a-112">说明</span><span class="sxs-lookup"><span data-stu-id="bb15a-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bb15a-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="bb15a-113">**appliesTo**</span></span> | <span data-ttu-id="bb15a-114">string</span><span class="sxs-lookup"><span data-stu-id="bb15a-114">string</span></span> |  <span data-ttu-id="bb15a-115">要分配许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="bb15a-115">The user role type to assign to license.</span></span> <span data-ttu-id="bb15a-116">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="bb15a-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="bb15a-117">**name**</span><span class="sxs-lookup"><span data-stu-id="bb15a-117">**name**</span></span> | <span data-ttu-id="bb15a-118">string</span><span class="sxs-lookup"><span data-stu-id="bb15a-118">string</span></span> |  <span data-ttu-id="bb15a-119">表示的用户帐户的域。</span><span class="sxs-lookup"><span data-stu-id="bb15a-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="bb15a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb15a-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
