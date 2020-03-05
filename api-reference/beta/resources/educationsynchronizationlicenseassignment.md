---
title: educationSynchronizationLicenseAssignment 资源类型
description: 表示要分配给用户帐户的许可证信息。 创建新用户帐户时，资源将用于设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5c806b451cc7f757da09927a5732426b0971f2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500189"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="4b673-104">educationSynchronizationLicenseAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b673-104">educationSynchronizationLicenseAssignment resource type</span></span>

<span data-ttu-id="4b673-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4b673-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b673-106">表示要分配给用户帐户的许可证信息。</span><span class="sxs-lookup"><span data-stu-id="4b673-106">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="4b673-107">创建新用户帐户时，资源将用于设置许可证分配。</span><span class="sxs-lookup"><span data-stu-id="4b673-107">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="4b673-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b673-108">Properties</span></span>

| <span data-ttu-id="4b673-109">属性</span><span class="sxs-lookup"><span data-stu-id="4b673-109">Property</span></span> | <span data-ttu-id="4b673-110">类型</span><span class="sxs-lookup"><span data-stu-id="4b673-110">Type</span></span> | <span data-ttu-id="4b673-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b673-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4b673-112">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="4b673-112">**appliesTo**</span></span> | <span data-ttu-id="4b673-113">string</span><span class="sxs-lookup"><span data-stu-id="4b673-113">string</span></span> | <span data-ttu-id="4b673-114">要分配给许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="4b673-114">The user role type to assign to license.</span></span> <span data-ttu-id="4b673-115">可取值为：`student`、`teacher`、`faculty`。</span><span class="sxs-lookup"><span data-stu-id="4b673-115">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="4b673-116">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="4b673-116">**skuIds**</span></span> | <span data-ttu-id="4b673-117">字符串集合</span><span class="sxs-lookup"><span data-stu-id="4b673-117">collection of strings</span></span> |  <span data-ttu-id="4b673-118">表示要分配的许可证的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="4b673-118">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="4b673-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b673-119">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
