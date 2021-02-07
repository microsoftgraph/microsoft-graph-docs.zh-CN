---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 555243468312b9c0eb63ee1bae37d2088da8b025
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134958"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="55a75-103">certificateAuthority 资源类型</span><span class="sxs-lookup"><span data-stu-id="55a75-103">certificateAuthority resource type</span></span>

<span data-ttu-id="55a75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55a75-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55a75-105">表示证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="55a75-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="55a75-106">属性</span><span class="sxs-lookup"><span data-stu-id="55a75-106">Properties</span></span>

| <span data-ttu-id="55a75-107">属性</span><span class="sxs-lookup"><span data-stu-id="55a75-107">Property</span></span>     | <span data-ttu-id="55a75-108">类型</span><span class="sxs-lookup"><span data-stu-id="55a75-108">Type</span></span>        | <span data-ttu-id="55a75-109">说明</span><span class="sxs-lookup"><span data-stu-id="55a75-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55a75-110">证书</span><span class="sxs-lookup"><span data-stu-id="55a75-110">certificate</span></span>|<span data-ttu-id="55a75-111">Binary</span><span class="sxs-lookup"><span data-stu-id="55a75-111">Binary</span></span>|<span data-ttu-id="55a75-112">必填。</span><span class="sxs-lookup"><span data-stu-id="55a75-112">Required.</span></span> <span data-ttu-id="55a75-113">base64 编码字符串，表示公共证书。</span><span class="sxs-lookup"><span data-stu-id="55a75-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="55a75-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="55a75-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="55a75-115">String</span><span class="sxs-lookup"><span data-stu-id="55a75-115">String</span></span>|<span data-ttu-id="55a75-116">证书吊销列表的 URL。</span><span class="sxs-lookup"><span data-stu-id="55a75-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="55a75-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="55a75-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="55a75-118">String</span><span class="sxs-lookup"><span data-stu-id="55a75-118">String</span></span>|<span data-ttu-id="55a75-119">该 URL 包含自上次创建完整证书撤销列表以来所有吊销的证书的列表。</span><span class="sxs-lookup"><span data-stu-id="55a75-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="55a75-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="55a75-120">isRootAuthority</span></span>|<span data-ttu-id="55a75-121">布尔</span><span class="sxs-lookup"><span data-stu-id="55a75-121">Boolean</span></span>|<span data-ttu-id="55a75-122">必填。</span><span class="sxs-lookup"><span data-stu-id="55a75-122">Required.</span></span> <span data-ttu-id="55a75-123">如果受信任证书是根证书颁发机构，则其为 **true;** 如果受信任证书是中间证书颁发机构，则其为 false。</span><span class="sxs-lookup"><span data-stu-id="55a75-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="55a75-124">issuer</span><span class="sxs-lookup"><span data-stu-id="55a75-124">issuer</span></span>|<span data-ttu-id="55a75-125">String</span><span class="sxs-lookup"><span data-stu-id="55a75-125">String</span></span>|<span data-ttu-id="55a75-126">根据证书值计算得出的证书 **颁发** 者。</span><span class="sxs-lookup"><span data-stu-id="55a75-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="55a75-127">只读。</span><span class="sxs-lookup"><span data-stu-id="55a75-127">Read-only.</span></span> |
|<span data-ttu-id="55a75-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="55a75-128">issuerSki</span></span>|<span data-ttu-id="55a75-129">String</span><span class="sxs-lookup"><span data-stu-id="55a75-129">String</span></span>|<span data-ttu-id="55a75-130">证书的主题密钥标识符，根据证书值 **计算** 。</span><span class="sxs-lookup"><span data-stu-id="55a75-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="55a75-131">只读。</span><span class="sxs-lookup"><span data-stu-id="55a75-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55a75-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55a75-132">JSON representation</span></span>

<span data-ttu-id="55a75-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55a75-133">The following is a JSON representation of the resource.</span></span>

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
