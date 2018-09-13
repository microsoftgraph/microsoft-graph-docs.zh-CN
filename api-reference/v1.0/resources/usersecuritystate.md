# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="a3850-101">userSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3850-101">userSecurityState resource type</span></span>

<span data-ttu-id="a3850-102">包含有关用户帐户的状态信息。</span><span class="sxs-lookup"><span data-stu-id="a3850-102">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="a3850-103">属性</span><span class="sxs-lookup"><span data-stu-id="a3850-103">Properties</span></span>

| <span data-ttu-id="a3850-104">属性</span><span class="sxs-lookup"><span data-stu-id="a3850-104">Property</span></span>   | <span data-ttu-id="a3850-105">类型</span><span class="sxs-lookup"><span data-stu-id="a3850-105">Type</span></span> |<span data-ttu-id="a3850-106">说明</span><span class="sxs-lookup"><span data-stu-id="a3850-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3850-107">aadUserId</span><span class="sxs-lookup"><span data-stu-id="a3850-107">aadUserId</span></span>|<span data-ttu-id="a3850-108">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-108">String</span></span>|<span data-ttu-id="a3850-109">AAD 用户对象标识符 (GUID) - 表示物理/多帐户用户实体。</span><span class="sxs-lookup"><span data-stu-id="a3850-109">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="a3850-110">accountName</span><span class="sxs-lookup"><span data-stu-id="a3850-110">accountName</span></span>|<span data-ttu-id="a3850-111">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-111">String</span></span>|<span data-ttu-id="a3850-112">用户帐户的帐户名称（没有 Active Directory 域和 DNS 域）- (也称为 `mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="a3850-112">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="a3850-113">domainName</span><span class="sxs-lookup"><span data-stu-id="a3850-113">domainName</span></span>|<span data-ttu-id="a3850-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-114">String</span></span>|<span data-ttu-id="a3850-115">用户帐户的 NetBIOS/Active Directory 域 （即域\帐户格式）。</span><span class="sxs-lookup"><span data-stu-id="a3850-115">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="a3850-116">emailRole</span><span class="sxs-lookup"><span data-stu-id="a3850-116">emailRole</span></span>|<span data-ttu-id="a3850-117">emailRole</span><span class="sxs-lookup"><span data-stu-id="a3850-117">emailRole</span></span>|<span data-ttu-id="a3850-118">与电子邮件相关的通知 - 用户帐户的电子邮件“角色”。</span><span class="sxs-lookup"><span data-stu-id="a3850-118">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="a3850-119">可取值为：`unknown`、`sender`、`recipient`。</span><span class="sxs-lookup"><span data-stu-id="a3850-119">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="a3850-120">isVpn</span><span class="sxs-lookup"><span data-stu-id="a3850-120">isVpn</span></span>|<span data-ttu-id="a3850-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="a3850-121">Boolean</span></span>|<span data-ttu-id="a3850-122">指示用户是否通过 VPN 登录。</span><span class="sxs-lookup"><span data-stu-id="a3850-122">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="a3850-123">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="a3850-123">logonDateTime</span></span>|<span data-ttu-id="a3850-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3850-124">DateTimeOffset</span></span>|<span data-ttu-id="a3850-125">登录发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a3850-125">Time at which the sign-in occurred.</span></span> <span data-ttu-id="a3850-126">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a3850-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a3850-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a3850-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a3850-128">logonId</span><span class="sxs-lookup"><span data-stu-id="a3850-128">logonId</span></span>|<span data-ttu-id="a3850-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-129">String</span></span>|<span data-ttu-id="a3850-130">用户登录 ID。</span><span class="sxs-lookup"><span data-stu-id="a3850-130">User sign-in ID.</span></span>|
|<span data-ttu-id="a3850-131">logonIp</span><span class="sxs-lookup"><span data-stu-id="a3850-131">logonIp</span></span>|<span data-ttu-id="a3850-132">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-132">String</span></span>|<span data-ttu-id="a3850-133">登录请求源自的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="a3850-133">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="a3850-134">logonLocation</span><span class="sxs-lookup"><span data-stu-id="a3850-134">logonLocation</span></span>|<span data-ttu-id="a3850-135">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-135">String</span></span>|<span data-ttu-id="a3850-136">此用户与用户登录事件关联的位置（通过 IP 地址映射）。</span><span class="sxs-lookup"><span data-stu-id="a3850-136">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="a3850-137">logonType</span><span class="sxs-lookup"><span data-stu-id="a3850-137">logonType</span></span>|<span data-ttu-id="a3850-138">logonType</span><span class="sxs-lookup"><span data-stu-id="a3850-138">logonType</span></span>|<span data-ttu-id="a3850-139">用户登录的方法。</span><span class="sxs-lookup"><span data-stu-id="a3850-139">Method of user sign in.</span></span> <span data-ttu-id="a3850-140">可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="a3850-140">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="a3850-141">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a3850-141">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="a3850-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-142">String</span></span>|<span data-ttu-id="a3850-143">用户的 Active Directory （本地）安全标识符 (SID)。</span><span class="sxs-lookup"><span data-stu-id="a3850-143">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="a3850-144">riskScore</span><span class="sxs-lookup"><span data-stu-id="a3850-144">riskScore</span></span>|<span data-ttu-id="a3850-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-145">String</span></span>|<span data-ttu-id="a3850-146">提供程序生成/计算的用户帐户风险评分。</span><span class="sxs-lookup"><span data-stu-id="a3850-146">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="a3850-147">建议值的范围为 0-1，相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="a3850-147">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="a3850-148">userAccountType</span><span class="sxs-lookup"><span data-stu-id="a3850-148">userAccountType</span></span>|<span data-ttu-id="a3850-149">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="a3850-149">userAccountSecurityType</span></span>|<span data-ttu-id="a3850-150">用户帐户类型 （组成员身份），依照 Windows 定义。</span><span class="sxs-lookup"><span data-stu-id="a3850-150">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="a3850-151">可取值为：`unknown`、`standard`、`power`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="a3850-151">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="a3850-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3850-152">userPrincipalName</span></span>|<span data-ttu-id="a3850-153">字符串</span><span class="sxs-lookup"><span data-stu-id="a3850-153">String</span></span>|<span data-ttu-id="a3850-154">用户登录名 - 互联网格式：（用户帐户名）@（用户帐户 DNS 域名）。</span><span class="sxs-lookup"><span data-stu-id="a3850-154">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3850-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3850-155">JSON representation</span></span>

<span data-ttu-id="a3850-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3850-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
