---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据, 然后再重新启动请求, 才能与 Azure Active Directory (Azure AD) 同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cf462873226ff4238f95ffc4798b6eb662666f3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006407"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="b482b-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b482b-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b482b-106">表示返回给客户端以响应对基于 CSV 的学校数据配置文件的[启动同步](../api/educationsynchronizationprofile-start.md)的请求的错误。</span><span class="sxs-lookup"><span data-stu-id="b482b-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="b482b-107">资源将包含验证导致的错误。</span><span class="sxs-lookup"><span data-stu-id="b482b-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="b482b-108">用户必须先修复源数据, 然后再重新启动请求, 才能与 Azure Active Directory (Azure AD) 同步。</span><span class="sxs-lookup"><span data-stu-id="b482b-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b482b-109">属性</span><span class="sxs-lookup"><span data-stu-id="b482b-109">Properties</span></span>

| <span data-ttu-id="b482b-110">属性</span><span class="sxs-lookup"><span data-stu-id="b482b-110">Property</span></span> | <span data-ttu-id="b482b-111">类型</span><span class="sxs-lookup"><span data-stu-id="b482b-111">Type</span></span> | <span data-ttu-id="b482b-112">说明</span><span class="sxs-lookup"><span data-stu-id="b482b-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b482b-113">**类型**</span><span class="sxs-lookup"><span data-stu-id="b482b-113">**type**</span></span> | <span data-ttu-id="b482b-114">string</span><span class="sxs-lookup"><span data-stu-id="b482b-114">string</span></span> | <span data-ttu-id="b482b-115">邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="b482b-115">Type of the message.</span></span> <span data-ttu-id="b482b-116">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="b482b-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="b482b-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="b482b-117">**filename**</span></span> | <span data-ttu-id="b482b-118">string</span><span class="sxs-lookup"><span data-stu-id="b482b-118">string</span></span> | <span data-ttu-id="b482b-119">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="b482b-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="b482b-120">**说明**</span><span class="sxs-lookup"><span data-stu-id="b482b-120">**description**</span></span> | <span data-ttu-id="b482b-121">string</span><span class="sxs-lookup"><span data-stu-id="b482b-121">string</span></span> | <span data-ttu-id="b482b-122">有关邮件类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b482b-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b482b-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b482b-123">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
