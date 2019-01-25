---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 代表向客户端启动基于 CSV 学校数据配置文件同步的请求的响应中返回的错误。 该资源将包含错误而形成了验证从。 重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529892"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="c3ce3-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3ce3-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ce3-106">代表向客户端基于 CSV 学校数据配置文件[启动同步](../api/educationsynchronizationprofile-start.md)到请求的响应中返回的错误。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="c3ce3-107">该资源将包含错误而形成了验证从。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="c3ce3-108">重新启动与 Azure Active Directory (Azure AD) 的同步请求之前，用户必须修复的源数据。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="c3ce3-109">属性</span><span class="sxs-lookup"><span data-stu-id="c3ce3-109">Properties</span></span>

| <span data-ttu-id="c3ce3-110">属性</span><span class="sxs-lookup"><span data-stu-id="c3ce3-110">Property</span></span> | <span data-ttu-id="c3ce3-111">类型</span><span class="sxs-lookup"><span data-stu-id="c3ce3-111">Type</span></span> | <span data-ttu-id="c3ce3-112">说明</span><span class="sxs-lookup"><span data-stu-id="c3ce3-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c3ce3-113">**类型**</span><span class="sxs-lookup"><span data-stu-id="c3ce3-113">**type**</span></span> | <span data-ttu-id="c3ce3-114">string</span><span class="sxs-lookup"><span data-stu-id="c3ce3-114">string</span></span> | <span data-ttu-id="c3ce3-115">消息的类型。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-115">Type of the message.</span></span> <span data-ttu-id="c3ce3-116">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="c3ce3-117">**fileName**</span><span class="sxs-lookup"><span data-stu-id="c3ce3-117">**filename**</span></span> | <span data-ttu-id="c3ce3-118">string</span><span class="sxs-lookup"><span data-stu-id="c3ce3-118">string</span></span> | <span data-ttu-id="c3ce3-119">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="c3ce3-120">**说明**</span><span class="sxs-lookup"><span data-stu-id="c3ce3-120">**description**</span></span> | <span data-ttu-id="c3ce3-121">string</span><span class="sxs-lookup"><span data-stu-id="c3ce3-121">string</span></span> | <span data-ttu-id="c3ce3-122">有关邮件类型的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="c3ce3-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3ce3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3ce3-123">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
