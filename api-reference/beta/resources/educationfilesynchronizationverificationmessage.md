---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507110"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="cffa6-105">educationFileSynchronizationVerificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="cffa6-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cffa6-106">表示返回给客户端以响应对基于 CSV 的学校数据配置文件的[启动同步](../api/educationsynchronizationprofile-start.md)的请求的错误。</span><span class="sxs-lookup"><span data-stu-id="cffa6-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="cffa6-107">资源将包含验证导致的错误。</span><span class="sxs-lookup"><span data-stu-id="cffa6-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="cffa6-108">用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。</span><span class="sxs-lookup"><span data-stu-id="cffa6-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="cffa6-109">属性</span><span class="sxs-lookup"><span data-stu-id="cffa6-109">Properties</span></span>

| <span data-ttu-id="cffa6-110">属性</span><span class="sxs-lookup"><span data-stu-id="cffa6-110">Property</span></span> | <span data-ttu-id="cffa6-111">类型</span><span class="sxs-lookup"><span data-stu-id="cffa6-111">Type</span></span> | <span data-ttu-id="cffa6-112">说明</span><span class="sxs-lookup"><span data-stu-id="cffa6-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cffa6-113">**类型**</span><span class="sxs-lookup"><span data-stu-id="cffa6-113">**type**</span></span> | <span data-ttu-id="cffa6-114">string</span><span class="sxs-lookup"><span data-stu-id="cffa6-114">string</span></span> | <span data-ttu-id="cffa6-115">邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="cffa6-115">Type of the message.</span></span> <span data-ttu-id="cffa6-116">可取值为：`error`、`warning`、`information`。</span><span class="sxs-lookup"><span data-stu-id="cffa6-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="cffa6-117">**filename**</span><span class="sxs-lookup"><span data-stu-id="cffa6-117">**filename**</span></span> | <span data-ttu-id="cffa6-118">字符串</span><span class="sxs-lookup"><span data-stu-id="cffa6-118">string</span></span> | <span data-ttu-id="cffa6-119">包含错误的源文件。</span><span class="sxs-lookup"><span data-stu-id="cffa6-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="cffa6-120">**说明**</span><span class="sxs-lookup"><span data-stu-id="cffa6-120">**description**</span></span> | <span data-ttu-id="cffa6-121">string</span><span class="sxs-lookup"><span data-stu-id="cffa6-121">string</span></span> | <span data-ttu-id="cffa6-122">有关邮件类型的详细信息。</span><span class="sxs-lookup"><span data-stu-id="cffa6-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cffa6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cffa6-123">JSON representation</span></span>

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
