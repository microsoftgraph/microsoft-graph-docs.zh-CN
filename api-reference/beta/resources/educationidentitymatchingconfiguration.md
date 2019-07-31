---
title: educationIdentityMatchingConfiguration 资源类型
description: 定义用于匹配学校数据配置文件标识的设置。 这些标识包括学生和教师。 根据这些设置, 将在目录中更新用户。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6805fabd857e4e906fa095c372632edbcc27fa28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006386"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="814b2-105">educationIdentityMatchingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="814b2-105">educationIdentityMatchingConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="814b2-106">定义用于匹配学校数据配置文件标识的设置。</span><span class="sxs-lookup"><span data-stu-id="814b2-106">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="814b2-107">这些标识包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="814b2-107">These identities include students and teachers.</span></span> <span data-ttu-id="814b2-108">根据这些设置, 将在目录中更新用户。</span><span class="sxs-lookup"><span data-stu-id="814b2-108">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="814b2-109">**注意:** 在选择此资源时不会创建任何用户。</span><span class="sxs-lookup"><span data-stu-id="814b2-109">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="814b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="814b2-110">Properties</span></span>

| <span data-ttu-id="814b2-111">属性</span><span class="sxs-lookup"><span data-stu-id="814b2-111">Property</span></span> | <span data-ttu-id="814b2-112">类型</span><span class="sxs-lookup"><span data-stu-id="814b2-112">Type</span></span> | <span data-ttu-id="814b2-113">说明</span><span class="sxs-lookup"><span data-stu-id="814b2-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="814b2-114">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="814b2-114">**matchingOptions**</span></span> | <span data-ttu-id="814b2-115">[educationIdentityMatchingOptions](educationidentitymatchingoptions.md)集合</span><span class="sxs-lookup"><span data-stu-id="814b2-115">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="814b2-116">用户帐户与用于唯一标识要更新的用户的选项之间的映射。</span><span class="sxs-lookup"><span data-stu-id="814b2-116">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="814b2-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="814b2-117">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
