---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
ms.openlocfilehash: f2826f779aac3ba41146b6677f3d1e0364be92a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336062"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="2c15d-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c15d-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="2c15d-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2c15d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c15d-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c15d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c15d-108">代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。</span><span class="sxs-lookup"><span data-stu-id="2c15d-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="2c15d-109">该资源将包含错误而形成了验证从。</span><span class="sxs-lookup"><span data-stu-id="2c15d-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="2c15d-110">重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。</span><span class="sxs-lookup"><span data-stu-id="2c15d-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="2c15d-111">属性</span><span class="sxs-lookup"><span data-stu-id="2c15d-111">Properties</span></span>

| <span data-ttu-id="2c15d-112">属性</span><span class="sxs-lookup"><span data-stu-id="2c15d-112">Property</span></span> | <span data-ttu-id="2c15d-113">类型</span><span class="sxs-lookup"><span data-stu-id="2c15d-113">Type</span></span> | <span data-ttu-id="2c15d-114">说明</span><span class="sxs-lookup"><span data-stu-id="2c15d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2c15d-115">**类型**</span><span class="sxs-lookup"><span data-stu-id="2c15d-115">**type**</span></span> | <span data-ttu-id="2c15d-116">string</span><span class="sxs-lookup"><span data-stu-id="2c15d-116">string</span></span> | <span data-ttu-id="2c15d-117">消息的类型。</span><span class="sxs-lookup"><span data-stu-id="2c15d-117">Type of the message.</span></span> <span data-ttu-id="2c15d-118">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="2c15d-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="2c15d-119">**文件名**</span><span class="sxs-lookup"><span data-stu-id="2c15d-119">**filename**</span></span> | <span data-ttu-id="2c15d-120">string</span><span class="sxs-lookup"><span data-stu-id="2c15d-120">string</span></span> | <span data-ttu-id="2c15d-121">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="2c15d-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="2c15d-122">**说明**</span><span class="sxs-lookup"><span data-stu-id="2c15d-122">**description**</span></span> | <span data-ttu-id="2c15d-123">string</span><span class="sxs-lookup"><span data-stu-id="2c15d-123">string</span></span> | <span data-ttu-id="2c15d-124">有关邮件类型的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="2c15d-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c15d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c15d-125">JSON representation</span></span>

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