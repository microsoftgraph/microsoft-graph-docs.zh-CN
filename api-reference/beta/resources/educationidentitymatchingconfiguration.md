---
title: educationIdentityMatchingConfiguration 资源类型
description: 用于匹配学校数据配置文件标识中定义的设置。 这些身份包括学生和教师。 根据这些设置，用户将更新目录中。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ded27e432219a247bf9c03c21f8ebd0054183eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411328"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a><span data-ttu-id="38bdd-105">educationIdentityMatchingConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="38bdd-105">educationIdentityMatchingConfiguration resource type</span></span>

> <span data-ttu-id="38bdd-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38bdd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38bdd-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38bdd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38bdd-108">用于匹配学校数据配置文件标识中定义的设置。</span><span class="sxs-lookup"><span data-stu-id="38bdd-108">Defines the settings for matching school data profile identities.</span></span> <span data-ttu-id="38bdd-109">这些身份包括学生和教师。</span><span class="sxs-lookup"><span data-stu-id="38bdd-109">These identities include students and teachers.</span></span> <span data-ttu-id="38bdd-110">根据这些设置，用户将更新目录中。</span><span class="sxs-lookup"><span data-stu-id="38bdd-110">Based on these settings, the users will be updated in the directory.</span></span>

> <span data-ttu-id="38bdd-111">**注意：** 选择此资源时，会不创建任何用户。</span><span class="sxs-lookup"><span data-stu-id="38bdd-111">**Note:** No users are created when this resource is selected.</span></span>

## <a name="properties"></a><span data-ttu-id="38bdd-112">属性</span><span class="sxs-lookup"><span data-stu-id="38bdd-112">Properties</span></span>

| <span data-ttu-id="38bdd-113">属性</span><span class="sxs-lookup"><span data-stu-id="38bdd-113">Property</span></span> | <span data-ttu-id="38bdd-114">类型</span><span class="sxs-lookup"><span data-stu-id="38bdd-114">Type</span></span> | <span data-ttu-id="38bdd-115">说明</span><span class="sxs-lookup"><span data-stu-id="38bdd-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="38bdd-116">**matchingOptions**</span><span class="sxs-lookup"><span data-stu-id="38bdd-116">**matchingOptions**</span></span> | <span data-ttu-id="38bdd-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md)集合</span><span class="sxs-lookup"><span data-stu-id="38bdd-117">[microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md) collection</span></span> | <span data-ttu-id="38bdd-118">用户帐户和选项用于唯一标识用户更新之间的映射。</span><span class="sxs-lookup"><span data-stu-id="38bdd-118">Mapping between the user account and the options to use to uniquely identify the user to update.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="38bdd-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38bdd-119">JSON representation</span></span>
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
