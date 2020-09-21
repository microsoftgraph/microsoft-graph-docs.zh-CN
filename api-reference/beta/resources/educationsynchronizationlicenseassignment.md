---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时，资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b5aea834ff2943046aff8a390ae110d775fd2f20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989638"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="8db6b-104">educationSynchronizationLicenseAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="8db6b-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="8db6b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8db6b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8db6b-106">表示要分配给用户帐户的许可证信息。</span><span class="sxs-lookup"><span data-stu-id="8db6b-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="8db6b-107">创建新用户帐户时，资源将用于设置许可证分配。</span><span class="sxs-lookup"><span data-stu-id="8db6b-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="8db6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8db6b-108">Properties</span></span>

| <span data-ttu-id="8db6b-109">属性</span><span class="sxs-lookup"><span data-stu-id="8db6b-109">Property</span></span>  | <span data-ttu-id="8db6b-110">类型</span><span class="sxs-lookup"><span data-stu-id="8db6b-110">Type</span></span>              | <span data-ttu-id="8db6b-111">说明</span><span class="sxs-lookup"><span data-stu-id="8db6b-111">Description</span></span>                                                                                    |
| :-------- | :---------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8db6b-112">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8db6b-112">appliesTo</span></span> | <span data-ttu-id="8db6b-113">String</span><span class="sxs-lookup"><span data-stu-id="8db6b-113">String</span></span>            | <span data-ttu-id="8db6b-114">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="8db6b-114">The user role type to assign to license.</span></span> <span data-ttu-id="8db6b-115">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="8db6b-115">Possible values are: `student`, `teacher`, `faculty`.</span></span> |
| <span data-ttu-id="8db6b-116">skuIds</span><span class="sxs-lookup"><span data-stu-id="8db6b-116">skuIds</span></span>    | <span data-ttu-id="8db6b-117">String collection</span><span class="sxs-lookup"><span data-stu-id="8db6b-117">String collection</span></span> | <span data-ttu-id="8db6b-118">表示要分配的许可证的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="8db6b-118">Represents the SKU identifiers of the licenses to assign.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="8db6b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8db6b-119">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
  "appliesTo": { "@odata.type": "microsoft.graph.educationUserRole" },
  "skuIds": ["String"]
}
```


