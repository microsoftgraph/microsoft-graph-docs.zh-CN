---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 030e0fbe8fcae0408f51c20882d49e50d825cdb8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539293"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="9493c-103">certificateAuthority 资源类型</span><span class="sxs-lookup"><span data-stu-id="9493c-103">certificateAuthority resource type</span></span>

<span data-ttu-id="9493c-104">表示证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="9493c-104">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="9493c-105">属性</span><span class="sxs-lookup"><span data-stu-id="9493c-105">Properties</span></span>

| <span data-ttu-id="9493c-106">属性</span><span class="sxs-lookup"><span data-stu-id="9493c-106">Property</span></span>     | <span data-ttu-id="9493c-107">类型</span><span class="sxs-lookup"><span data-stu-id="9493c-107">Type</span></span>        | <span data-ttu-id="9493c-108">说明</span><span class="sxs-lookup"><span data-stu-id="9493c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9493c-109">证书</span><span class="sxs-lookup"><span data-stu-id="9493c-109">certificate</span></span>|<span data-ttu-id="9493c-110">Binary</span><span class="sxs-lookup"><span data-stu-id="9493c-110">Binary</span></span>|<span data-ttu-id="9493c-111">必需。</span><span class="sxs-lookup"><span data-stu-id="9493c-111">Required.</span></span> <span data-ttu-id="9493c-112">表示公共证书的 base64 编码字符串。</span><span class="sxs-lookup"><span data-stu-id="9493c-112">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="9493c-113">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="9493c-113">certificateRevocationListUrl</span></span>|<span data-ttu-id="9493c-114">字符串</span><span class="sxs-lookup"><span data-stu-id="9493c-114">String</span></span>|<span data-ttu-id="9493c-115">证书吊销列表的 URL。</span><span class="sxs-lookup"><span data-stu-id="9493c-115">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="9493c-116">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="9493c-116">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="9493c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="9493c-117">String</span></span>|<span data-ttu-id="9493c-118">该 URL 包含自上次创建完整证书 revocaton 列表以来的所有已吊销证书的列表。</span><span class="sxs-lookup"><span data-stu-id="9493c-118">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="9493c-119">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="9493c-119">isRootAuthority</span></span>|<span data-ttu-id="9493c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="9493c-120">Boolean</span></span>|<span data-ttu-id="9493c-121">必需。</span><span class="sxs-lookup"><span data-stu-id="9493c-121">Required.</span></span> <span data-ttu-id="9493c-122">如果受信任的证书是根证书颁发机构，**则为 true** ; 如果受信任的证书是中间颁发机构，则为**false** 。</span><span class="sxs-lookup"><span data-stu-id="9493c-122">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="9493c-123">常用</span><span class="sxs-lookup"><span data-stu-id="9493c-123">issuer</span></span>|<span data-ttu-id="9493c-124">字符串</span><span class="sxs-lookup"><span data-stu-id="9493c-124">String</span></span>|<span data-ttu-id="9493c-125">证书的颁发者，根据**证书**值计算。</span><span class="sxs-lookup"><span data-stu-id="9493c-125">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="9493c-126">只读。</span><span class="sxs-lookup"><span data-stu-id="9493c-126">Read-only.</span></span> |
|<span data-ttu-id="9493c-127">issuerSki</span><span class="sxs-lookup"><span data-stu-id="9493c-127">issuerSki</span></span>|<span data-ttu-id="9493c-128">字符串</span><span class="sxs-lookup"><span data-stu-id="9493c-128">String</span></span>|<span data-ttu-id="9493c-129">证书的主题密钥标识符，由**证书**值计算得出。</span><span class="sxs-lookup"><span data-stu-id="9493c-129">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="9493c-130">只读。</span><span class="sxs-lookup"><span data-stu-id="9493c-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9493c-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9493c-131">JSON representation</span></span>

<span data-ttu-id="9493c-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9493c-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->