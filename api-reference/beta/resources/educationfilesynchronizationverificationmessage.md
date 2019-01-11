---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845512"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="5114e-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="5114e-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="5114e-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5114e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5114e-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5114e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5114e-108">代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。</span><span class="sxs-lookup"><span data-stu-id="5114e-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="5114e-109">该资源将包含错误而形成了验证从。</span><span class="sxs-lookup"><span data-stu-id="5114e-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="5114e-110">重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。</span><span class="sxs-lookup"><span data-stu-id="5114e-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="5114e-111">属性</span><span class="sxs-lookup"><span data-stu-id="5114e-111">Properties</span></span>

| <span data-ttu-id="5114e-112">属性</span><span class="sxs-lookup"><span data-stu-id="5114e-112">Property</span></span> | <span data-ttu-id="5114e-113">类型</span><span class="sxs-lookup"><span data-stu-id="5114e-113">Type</span></span> | <span data-ttu-id="5114e-114">说明</span><span class="sxs-lookup"><span data-stu-id="5114e-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5114e-115">**类型**</span><span class="sxs-lookup"><span data-stu-id="5114e-115">**type**</span></span> | <span data-ttu-id="5114e-116">string</span><span class="sxs-lookup"><span data-stu-id="5114e-116">string</span></span> | <span data-ttu-id="5114e-117">消息的类型。</span><span class="sxs-lookup"><span data-stu-id="5114e-117">Type of the message.</span></span> <span data-ttu-id="5114e-118">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="5114e-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="5114e-119">**文件名**</span><span class="sxs-lookup"><span data-stu-id="5114e-119">**filename**</span></span> | <span data-ttu-id="5114e-120">string</span><span class="sxs-lookup"><span data-stu-id="5114e-120">string</span></span> | <span data-ttu-id="5114e-121">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="5114e-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="5114e-122">**说明**</span><span class="sxs-lookup"><span data-stu-id="5114e-122">**description**</span></span> | <span data-ttu-id="5114e-123">string</span><span class="sxs-lookup"><span data-stu-id="5114e-123">string</span></span> | <span data-ttu-id="5114e-124">有关邮件类型的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="5114e-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5114e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5114e-125">JSON representation</span></span>

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
