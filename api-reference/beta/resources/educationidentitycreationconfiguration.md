---
title: educationIdentityCreationConfiguration 资源类型
description: 定义有关创建学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置，将在目录中创建用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80c564999ca0e414c6475f858c5d3ebe5e037e4b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336020"
---
# <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="50a72-105">educationIdentityCreationConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="50a72-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50a72-106">定义有关创建学校数据配置文件标识的设置。</span><span class="sxs-lookup"><span data-stu-id="50a72-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="50a72-107">这些标识包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="50a72-107">These identities include students and teachers.</span></span> <span data-ttu-id="50a72-108">根据这些设置，将在目录中创建用户。</span><span class="sxs-lookup"><span data-stu-id="50a72-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="50a72-109">**注意：** 如果你打开了目录同步以在本地 Active Directory 和 Azure Active Directory （Azure AD）之间同步，请改用[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)资源。</span><span class="sxs-lookup"><span data-stu-id="50a72-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="50a72-110">派生自[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="50a72-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="50a72-111">属性</span><span class="sxs-lookup"><span data-stu-id="50a72-111">Properties</span></span>

| <span data-ttu-id="50a72-112">属性</span><span class="sxs-lookup"><span data-stu-id="50a72-112">Property</span></span> | <span data-ttu-id="50a72-113">类型</span><span class="sxs-lookup"><span data-stu-id="50a72-113">Type</span></span> | <span data-ttu-id="50a72-114">Description</span><span class="sxs-lookup"><span data-stu-id="50a72-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="50a72-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="50a72-115">**userDomains**</span></span> | <span data-ttu-id="50a72-116">[educationIdentityDomain](educationidentitydomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="50a72-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="50a72-117">设置要使用的每个用户类型的域的列表。</span><span class="sxs-lookup"><span data-stu-id="50a72-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="50a72-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50a72-118">JSON representation</span></span>
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
