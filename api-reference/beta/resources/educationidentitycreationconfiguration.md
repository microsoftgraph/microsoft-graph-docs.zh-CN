---
title: educationIdentityCreationConfiguration 资源类型
description: 定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置, 将在目录中创建用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507159"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="7345d-105">educationIdentityCreationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7345d-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7345d-106">定义有关创建学校数据配置文件标识的设置。</span><span class="sxs-lookup"><span data-stu-id="7345d-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="7345d-107">这些标识包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="7345d-107">These identities include students and teachers.</span></span> <span data-ttu-id="7345d-108">根据这些设置, 将在目录中创建用户。</span><span class="sxs-lookup"><span data-stu-id="7345d-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="7345d-109">**注意:** 如果你打开了目录同步以在本地 Active directory 和 azure Active directory (azure AD) 之间同步, 请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。</span><span class="sxs-lookup"><span data-stu-id="7345d-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="7345d-110">派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="7345d-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7345d-111">属性</span><span class="sxs-lookup"><span data-stu-id="7345d-111">Properties</span></span>

| <span data-ttu-id="7345d-112">属性</span><span class="sxs-lookup"><span data-stu-id="7345d-112">Property</span></span> | <span data-ttu-id="7345d-113">类型</span><span class="sxs-lookup"><span data-stu-id="7345d-113">Type</span></span> | <span data-ttu-id="7345d-114">说明</span><span class="sxs-lookup"><span data-stu-id="7345d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7345d-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="7345d-115">**userDomains**</span></span> | <span data-ttu-id="7345d-116">[educationIdentityDomain](educationidentitydomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="7345d-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="7345d-117">设置要使用的每个用户类型的域的列表。</span><span class="sxs-lookup"><span data-stu-id="7345d-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="7345d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7345d-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
