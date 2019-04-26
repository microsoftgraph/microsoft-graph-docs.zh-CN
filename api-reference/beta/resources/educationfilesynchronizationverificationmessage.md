---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bbf38f15fbe14112ef254c625a8747e57eb1cae4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340509"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="15ff5-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="15ff5-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ff5-106">表示返回给客户端以响应对基于 CSV 的学校数据配置文件的[启动同步](../api/educationsynchronizationprofile-start.md)的请求的错误。</span><span class="sxs-lookup"><span data-stu-id="15ff5-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="15ff5-107">资源将包含验证导致的错误。</span><span class="sxs-lookup"><span data-stu-id="15ff5-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="15ff5-108">用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。</span><span class="sxs-lookup"><span data-stu-id="15ff5-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="15ff5-109">属性</span><span class="sxs-lookup"><span data-stu-id="15ff5-109">Properties</span></span>

| <span data-ttu-id="15ff5-110">属性</span><span class="sxs-lookup"><span data-stu-id="15ff5-110">Property</span></span> | <span data-ttu-id="15ff5-111">类型</span><span class="sxs-lookup"><span data-stu-id="15ff5-111">Type</span></span> | <span data-ttu-id="15ff5-112">说明</span><span class="sxs-lookup"><span data-stu-id="15ff5-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="15ff5-113">**类型**</span><span class="sxs-lookup"><span data-stu-id="15ff5-113">**type**</span></span> | <span data-ttu-id="15ff5-114">string</span><span class="sxs-lookup"><span data-stu-id="15ff5-114">string</span></span> | <span data-ttu-id="15ff5-115">邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="15ff5-115">Type of the message.</span></span> <span data-ttu-id="15ff5-116">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="15ff5-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="15ff5-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="15ff5-117">**filename**</span></span> | <span data-ttu-id="15ff5-118">string</span><span class="sxs-lookup"><span data-stu-id="15ff5-118">string</span></span> | <span data-ttu-id="15ff5-119">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="15ff5-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="15ff5-120">**说明**</span><span class="sxs-lookup"><span data-stu-id="15ff5-120">**description**</span></span> | <span data-ttu-id="15ff5-121">string</span><span class="sxs-lookup"><span data-stu-id="15ff5-121">string</span></span> | <span data-ttu-id="15ff5-122">有关邮件类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="15ff5-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="15ff5-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15ff5-123">JSON representation</span></span>

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
