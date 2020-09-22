---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据，然后再重新启动请求，才能与 Azure Active Directory (Azure AD) 同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b65335538453f35457d5e83c49f7ba7c830d6a43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095436"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="72d02-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="72d02-105">educationFileSynchronizationVerificationMessage resource type</span></span>

<span data-ttu-id="72d02-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d02-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d02-107">表示返回给客户端以响应对基于 CSV 的学校数据配置文件的 [启动同步](../api/educationsynchronizationprofile-start.md) 的请求的错误。</span><span class="sxs-lookup"><span data-stu-id="72d02-107">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="72d02-108">资源将包含验证导致的错误。</span><span class="sxs-lookup"><span data-stu-id="72d02-108">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="72d02-109">用户必须先修复源数据，然后再重新启动请求，才能与 Azure Active Directory (Azure AD) 同步。</span><span class="sxs-lookup"><span data-stu-id="72d02-109">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="72d02-110">属性</span><span class="sxs-lookup"><span data-stu-id="72d02-110">Properties</span></span>

| <span data-ttu-id="72d02-111">属性</span><span class="sxs-lookup"><span data-stu-id="72d02-111">Property</span></span>    | <span data-ttu-id="72d02-112">类型</span><span class="sxs-lookup"><span data-stu-id="72d02-112">Type</span></span>   | <span data-ttu-id="72d02-113">说明</span><span class="sxs-lookup"><span data-stu-id="72d02-113">Description</span></span>                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="72d02-114">类型</span><span class="sxs-lookup"><span data-stu-id="72d02-114">type</span></span>        | <span data-ttu-id="72d02-115">string</span><span class="sxs-lookup"><span data-stu-id="72d02-115">string</span></span> | <span data-ttu-id="72d02-116">邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="72d02-116">Type of the message.</span></span> <span data-ttu-id="72d02-117">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="72d02-117">Possible values are: `error`, `warning`, `information`.</span></span> |
| <span data-ttu-id="72d02-118">filename</span><span class="sxs-lookup"><span data-stu-id="72d02-118">filename</span></span>    | <span data-ttu-id="72d02-119">string</span><span class="sxs-lookup"><span data-stu-id="72d02-119">string</span></span> | <span data-ttu-id="72d02-120">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="72d02-120">Source file that contains the error.</span></span>                                         |
| <span data-ttu-id="72d02-121">说明</span><span class="sxs-lookup"><span data-stu-id="72d02-121">description</span></span> | <span data-ttu-id="72d02-122">string</span><span class="sxs-lookup"><span data-stu-id="72d02-122">string</span></span> | <span data-ttu-id="72d02-123">有关邮件类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="72d02-123">Detailed information about the message type.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="72d02-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72d02-124">JSON representation</span></span>

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


