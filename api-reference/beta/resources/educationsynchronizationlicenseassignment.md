---
title: educationSynchronizationLicenseAssignment 资源类型
description: 代表分配给用户帐户的许可信息。 该资源将用于创建新的用户帐户时设置许可证分配。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 757e080a8b2c6f3f01fa1663f10c9b0b98eaf4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948273"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="3f866-104">educationSynchronizationLicenseAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f866-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="3f866-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3f866-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f866-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3f866-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f866-107">代表分配给用户帐户的许可信息。</span><span class="sxs-lookup"><span data-stu-id="3f866-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="3f866-108">该资源将用于创建新的用户帐户时设置许可证分配。</span><span class="sxs-lookup"><span data-stu-id="3f866-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="3f866-109">属性</span><span class="sxs-lookup"><span data-stu-id="3f866-109">Properties</span></span>

| <span data-ttu-id="3f866-110">属性</span><span class="sxs-lookup"><span data-stu-id="3f866-110">Property</span></span> | <span data-ttu-id="3f866-111">类型</span><span class="sxs-lookup"><span data-stu-id="3f866-111">Type</span></span> | <span data-ttu-id="3f866-112">Description</span><span class="sxs-lookup"><span data-stu-id="3f866-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3f866-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="3f866-113">**appliesTo**</span></span> | <span data-ttu-id="3f866-114">string</span><span class="sxs-lookup"><span data-stu-id="3f866-114">string</span></span> | <span data-ttu-id="3f866-115">要分配许可证的用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="3f866-115">The user role type to assign to license.</span></span> <span data-ttu-id="3f866-116">可取值为：`student`、`teacher`。</span><span class="sxs-lookup"><span data-stu-id="3f866-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="3f866-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="3f866-117">**skuIds**</span></span> | <span data-ttu-id="3f866-118">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3f866-118">collection of strings</span></span> |  <span data-ttu-id="3f866-119">表示分配的许可证的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="3f866-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="3f866-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f866-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
