---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cda1d5d3ac56c50cdeb94ada091e8ae2975b8813
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914477"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="d1eac-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1eac-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="d1eac-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1eac-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1eac-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1eac-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1eac-108">代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。</span><span class="sxs-lookup"><span data-stu-id="d1eac-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="d1eac-109">该资源将包含错误而形成了验证从。</span><span class="sxs-lookup"><span data-stu-id="d1eac-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="d1eac-110">重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。</span><span class="sxs-lookup"><span data-stu-id="d1eac-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="d1eac-111">属性</span><span class="sxs-lookup"><span data-stu-id="d1eac-111">Properties</span></span>

| <span data-ttu-id="d1eac-112">属性</span><span class="sxs-lookup"><span data-stu-id="d1eac-112">Property</span></span> | <span data-ttu-id="d1eac-113">类型</span><span class="sxs-lookup"><span data-stu-id="d1eac-113">Type</span></span> | <span data-ttu-id="d1eac-114">说明</span><span class="sxs-lookup"><span data-stu-id="d1eac-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d1eac-115">**类型**</span><span class="sxs-lookup"><span data-stu-id="d1eac-115">**type**</span></span> | <span data-ttu-id="d1eac-116">string</span><span class="sxs-lookup"><span data-stu-id="d1eac-116">string</span></span> | <span data-ttu-id="d1eac-117">消息的类型。</span><span class="sxs-lookup"><span data-stu-id="d1eac-117">Type of the message.</span></span> <span data-ttu-id="d1eac-118">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="d1eac-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="d1eac-119">**文件名**</span><span class="sxs-lookup"><span data-stu-id="d1eac-119">**filename**</span></span> | <span data-ttu-id="d1eac-120">string</span><span class="sxs-lookup"><span data-stu-id="d1eac-120">string</span></span> | <span data-ttu-id="d1eac-121">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="d1eac-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="d1eac-122">**说明**</span><span class="sxs-lookup"><span data-stu-id="d1eac-122">**description**</span></span> | <span data-ttu-id="d1eac-123">string</span><span class="sxs-lookup"><span data-stu-id="d1eac-123">string</span></span> | <span data-ttu-id="d1eac-124">有关邮件类型的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="d1eac-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1eac-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1eac-125">JSON representation</span></span>

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
