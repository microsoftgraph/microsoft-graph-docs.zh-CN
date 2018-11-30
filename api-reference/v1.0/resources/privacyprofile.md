---
title: privacyProfile 资源类型
description: 表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。
ms.openlocfilehash: 5d1a8e48a2d8310f45c71fbc73485e8ec4fe8697
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011111"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="00d58-103">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="00d58-103">privacyProfile resource type</span></span>

<span data-ttu-id="00d58-104">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="00d58-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="00d58-105">属性</span><span class="sxs-lookup"><span data-stu-id="00d58-105">Properties</span></span>
| <span data-ttu-id="00d58-106">属性</span><span class="sxs-lookup"><span data-stu-id="00d58-106">Property</span></span>   | <span data-ttu-id="00d58-107">类型</span><span class="sxs-lookup"><span data-stu-id="00d58-107">Type</span></span>|<span data-ttu-id="00d58-108">说明</span><span class="sxs-lookup"><span data-stu-id="00d58-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00d58-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="00d58-109">contactEmail</span></span>|<span data-ttu-id="00d58-110">String</span><span class="sxs-lookup"><span data-stu-id="00d58-110">String</span></span>| <span data-ttu-id="00d58-111">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="00d58-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="00d58-112">可选。</span><span class="sxs-lookup"><span data-stu-id="00d58-112">Not required.</span></span>|
|<span data-ttu-id="00d58-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="00d58-113">statementUrl</span></span>|<span data-ttu-id="00d58-114">String</span><span class="sxs-lookup"><span data-stu-id="00d58-114">String</span></span>| <span data-ttu-id="00d58-115">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="00d58-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="00d58-116">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="00d58-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="00d58-117">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="00d58-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="00d58-118">可选。</span><span class="sxs-lookup"><span data-stu-id="00d58-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00d58-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00d58-119">JSON representation</span></span>

<span data-ttu-id="00d58-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00d58-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```