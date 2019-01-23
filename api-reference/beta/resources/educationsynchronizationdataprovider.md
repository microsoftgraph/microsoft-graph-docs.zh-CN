---
title: educationSynchronizationDataProvider 资源类型
description: '代表源 SI 架构。 这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f1e51bd0039b28aa08fa71956efc5143df77651c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420967"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="97c87-104">educationSynchronizationDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="97c87-104">educationSynchronizationDataProvider resource type</span></span>

> <span data-ttu-id="97c87-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97c87-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97c87-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97c87-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97c87-107">代表源 SI 架构。</span><span class="sxs-lookup"><span data-stu-id="97c87-107">Represents the source SIS schema.</span></span> <span data-ttu-id="97c87-108">这样，系统以了解如何将传入的数据映射到 Azure Active Directory (Azure AD) 架构。</span><span class="sxs-lookup"><span data-stu-id="97c87-108">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span> 

> <span data-ttu-id="97c87-109">**注意：** 此复杂类型是抽象类。</span><span class="sxs-lookup"><span data-stu-id="97c87-109">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="97c87-110">引用的特定类型的数据提供程序列出。</span><span class="sxs-lookup"><span data-stu-id="97c87-110">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="97c87-111">派生的类型</span><span class="sxs-lookup"><span data-stu-id="97c87-111">Derived types</span></span>
| <span data-ttu-id="97c87-112">类型</span><span class="sxs-lookup"><span data-stu-id="97c87-112">Type</span></span> | <span data-ttu-id="97c87-113">说明</span><span class="sxs-lookup"><span data-stu-id="97c87-113">Description</span></span> | 
|:-|:-|:-|
| [<span data-ttu-id="97c87-114">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="97c87-114">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="97c87-115">作为输入源用于 CSV 文件。</span><span class="sxs-lookup"><span data-stu-id="97c87-115">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="97c87-116">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="97c87-116">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="97c87-117">用于 PowerSchool 作为输入源。</span><span class="sxs-lookup"><span data-stu-id="97c87-117">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="97c87-118">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="97c87-118">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="97c87-119">作为输入源用于 OneRoster API。</span><span class="sxs-lookup"><span data-stu-id="97c87-119">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="97c87-120">属性</span><span class="sxs-lookup"><span data-stu-id="97c87-120">Properties</span></span>

<span data-ttu-id="97c87-121">此类型不公开的任何属性。</span><span class="sxs-lookup"><span data-stu-id="97c87-121">No properties are exposed by this type.</span></span>



<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider "
}-->

```json
{
}
```
