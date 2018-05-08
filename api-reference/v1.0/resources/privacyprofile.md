# <a name="privacyprofile-resource-type"></a><span data-ttu-id="737b2-101">privacyProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="737b2-101">privacyProfile resource type</span></span>

<span data-ttu-id="737b2-102">表示公司的隐私配置文件，其中包括隐私声明 URL 和与隐私声明有关的联系人。</span><span class="sxs-lookup"><span data-stu-id="737b2-102">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="737b2-103">属性</span><span class="sxs-lookup"><span data-stu-id="737b2-103">Properties</span></span>
| <span data-ttu-id="737b2-104">属性</span><span class="sxs-lookup"><span data-stu-id="737b2-104">Property</span></span>   | <span data-ttu-id="737b2-105">类型</span><span class="sxs-lookup"><span data-stu-id="737b2-105">Type</span></span>|<span data-ttu-id="737b2-106">说明</span><span class="sxs-lookup"><span data-stu-id="737b2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="737b2-107">contactEmail</span><span class="sxs-lookup"><span data-stu-id="737b2-107">contactEmail</span></span>|<span data-ttu-id="737b2-108">String</span><span class="sxs-lookup"><span data-stu-id="737b2-108">String</span></span>| <span data-ttu-id="737b2-109">隐私声明联系人的有效 smtp 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="737b2-109">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="737b2-110">可选。</span><span class="sxs-lookup"><span data-stu-id="737b2-110">Not required</span></span>|
|<span data-ttu-id="737b2-111">statementUrl</span><span class="sxs-lookup"><span data-stu-id="737b2-111">statementUrl</span></span>|<span data-ttu-id="737b2-112">String</span><span class="sxs-lookup"><span data-stu-id="737b2-112">String</span></span>| <span data-ttu-id="737b2-113">以 http:// 或 https:// 开头的有效 URL 格式。</span><span class="sxs-lookup"><span data-stu-id="737b2-113">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="737b2-114">最大长度为 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="737b2-114">The maximum length is 255 characters.</span></span> <span data-ttu-id="737b2-115">定向到公司隐私声明的 URL。</span><span class="sxs-lookup"><span data-stu-id="737b2-115">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="737b2-116">可选。</span><span class="sxs-lookup"><span data-stu-id="737b2-116">Not required</span></span>|

## <a name="json-representation"></a><span data-ttu-id="737b2-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="737b2-117">JSON representation</span></span>

<span data-ttu-id="737b2-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="737b2-118">Here is a JSON representation of the resource</span></span>

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