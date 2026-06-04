# Reference
## Billing EstimateCharges
<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">list_estimate_charges</a>(...) -> EstimateChargesListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.list_estimate_charges()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_patient_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.patientId="pat_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_service_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.serviceId="svc_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_service_eligibility_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.serviceEligibilityId="sel_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_status:** `typing.Optional[EstimateChargesListV1FilterStatus]` — should be JSON-encoded, for example filter.status="AUTHORIZED"
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">create_estimate_charge</a>(...) -> EstimateChargeCreateV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.create_estimate_charge(
    patient_id="patientId",
    service_eligibility_id="serviceEligibilityId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `EstimateChargeCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">authorize_stripe_estimate_charge</a>(...) -> EstimateChargeAuthorizeStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.authorize_stripe_estimate_charge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">capture_stripe_estimate_charge</a>(...) -> EstimateChargeCaptureStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.capture_stripe_estimate_charge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">refund_stripe_estimate_charge</a>(...) -> EstimateChargeRefundStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.refund_stripe_estimate_charge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.estimate_charges.<a href="src/usebridge_api/billing/estimate_charges/client.py">cancel_stripe_estimate_charge</a>(...) -> EstimateChargeCancelStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.estimate_charges.cancel_stripe_estimate_charge(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Billing Fees
<details><summary><code>client.billing.fees.<a href="src/usebridge_api/billing/fees/client.py">list_fees</a>(...) -> FeesListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.fees.list_fees()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_patient_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.patientId="pat_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_service_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.serviceId="svc_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_service_eligibility_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.serviceEligibilityId="sel_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_status:** `typing.Optional[FeesListV1FilterStatus]` — should be JSON-encoded, for example filter.status="PENDING"
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.fees.<a href="src/usebridge_api/billing/fees/client.py">create_fee</a>(...) -> FeeCreateV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.fees.create_fee(
    patient_id="patientId",
    type="LATE_CANCELLATION",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `FeeCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.fees.<a href="src/usebridge_api/billing/fees/client.py">capture_stripe_fee</a>(...) -> FeeCaptureStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.fees.capture_stripe_fee(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.billing.fees.<a href="src/usebridge_api/billing/fees/client.py">refund_stripe_fee</a>(...) -> FeeRefundStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.fees.refund_stripe_fee(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Billing SetupIntent
<details><summary><code>client.billing.setup_intent.<a href="src/usebridge_api/billing/setup_intent/client.py">create_stripe_setup_intent</a>(...) -> SetupIntentCreateStripeV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint can only be used after setting up the billing integration. Refer to the [billing integration documentation](/documentation/integrations/billing/overview) for more details.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.billing.setup_intent.create_stripe_setup_intent(
    patient_id="patientId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `SetupIntentCreateStripeV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ConsentVersions
<details><summary><code>client.consent_versions.<a href="src/usebridge_api/consent_versions/client.py">list_consent_versions</a>(...) -> ConsentVersionsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.consent_versions.list_consent_versions()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Consent
<details><summary><code>client.consent.<a href="src/usebridge_api/consent/client.py">list_patient_consents</a>(...) -> PatientConsentsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.consent.list_patient_consents(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.consent.<a href="src/usebridge_api/consent/client.py">create_patient_consent</a>(...) -> PatientConsentCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.consent.create_patient_consent(
    id="id",
    type="ASSIGNMENT_OF_BENEFITS",
    version="version",
    consented_at=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `PatientConsentCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Events
<details><summary><code>client.events.<a href="src/usebridge_api/events/client.py">list_events</a>(...) -> EventsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.events.list_events()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_event_type:** `typing.Optional[str]` — Values should be JSON-encoded, for example filter.eventType="patient.created"
    
</dd>
</dl>

<dl>
<dd>

**filter_object_type:** `typing.Optional[str]` — Values should be JSON-encoded, for example filter.objectType="Patient"
    
</dd>
</dl>

<dl>
<dd>

**filter_object_id:** `typing.Optional[str]` — Values should be JSON-encoded, for example filter.objectId="pol_xxx"
    
</dd>
</dl>

<dl>
<dd>

**order_created_at:** `typing.Optional[EventsListV1OrderCreatedAt]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.events.<a href="src/usebridge_api/events/client.py">get_event</a>(...) -> EventGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.events.get_event(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Notes
<details><summary><code>client.notes.<a href="src/usebridge_api/notes/client.py">create_note</a>(...) -> NoteCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
from usebridge_api.notes import NoteCreateV1RequestData, NoteCreateV1RequestSignature
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.notes.create_note(
    service_id="serviceId",
    data=NoteCreateV1RequestData(),
    signature=NoteCreateV1RequestSignature(
        timestamp=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
        provider_id="providerId",
    ),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `NoteCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notes.<a href="src/usebridge_api/notes/client.py">get_note</a>(...) -> NoteGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.notes.get_note(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notes.<a href="src/usebridge_api/notes/client.py">list_note_addenda</a>(...) -> NoteAddendaListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.notes.list_note_addenda(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**filter_note_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.noteId="note_xxx"
    
</dd>
</dl>

<dl>
<dd>

**order_created_at:** `typing.Optional[NoteAddendaListV1OrderCreatedAt]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.notes.<a href="src/usebridge_api/notes/client.py">create_note_addendum</a>(...) -> NoteAddendumCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
from usebridge_api.notes import NoteAddendumCreateV1RequestData, NoteAddendumCreateV1RequestSignature
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.notes.create_note_addendum(
    id="id",
    data=NoteAddendumCreateV1RequestData(),
    signature=NoteAddendumCreateV1RequestSignature(
        timestamp=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
        provider_id="providerId",
    ),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `NoteAddendumCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## PatientToken
<details><summary><code>client.patient_token.<a href="src/usebridge_api/patient_token/client.py">create_patient_token</a>(...) -> PatientTokenCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patient_token.create_patient_token(
    patient_id="patientId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `PatientTokenCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Patients
<details><summary><code>client.patients.<a href="src/usebridge_api/patients/client.py">stream_patient</a>(...) -> typing.Iterator[bytes]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.stream_patient(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.patients.<a href="src/usebridge_api/patients/client.py">list_patients</a>(...) -> PatientsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.list_patients()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.patients.<a href="src/usebridge_api/patients/client.py">update_patient</a>(...) -> PatientUpdateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.update_patient(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `PatientUpdateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.patients.<a href="src/usebridge_api/patients/client.py">revalidate_patient</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.revalidate_patient(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Patients V2
<details><summary><code>client.patients.v_2.<a href="src/usebridge_api/patients/v_2/client.py">create_patient</a>(...) -> PatientCreateV2Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.v_2.create_patient(
    first_name="firstName",
    last_name="lastName",
    email="email",
    date_of_birth=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `PatientCreateV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.patients.v_2.<a href="src/usebridge_api/patients/v_2/client.py">get_patient</a>(...) -> PatientGetV2Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Resolves a Patient by either `id` or `externalId`
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.patients.v_2.get_patient(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## PayerGroups
<details><summary><code>client.payer_groups.<a href="src/usebridge_api/payer_groups/client.py">list_payer_groups</a>(...) -> PayerGroupsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payer_groups.list_payer_groups()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payer_groups.<a href="src/usebridge_api/payer_groups/client.py">get_payer_group</a>(...) -> PayerGroupGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payer_groups.get_payer_group(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Payer group ID or slug (both are supported)
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## PayerGroups Health
<details><summary><code>client.payer_groups.health.<a href="src/usebridge_api/payer_groups/health/client.py">list_health_events</a>(...) -> HealthEventsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payer_groups.health.list_health_events(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` — Payer group ID or slug (both are supported)
    
</dd>
</dl>

<dl>
<dd>

**order_event_at:** `typing.Optional[HealthEventsListV1OrderEventAt]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Payers
<details><summary><code>client.payers.<a href="src/usebridge_api/payers/client.py">get_payer</a>(...) -> PayerGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payers.get_payer(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Payments
<details><summary><code>client.payments.<a href="src/usebridge_api/payments/client.py">list_payments</a>(...) -> PaymentsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payments.list_payments()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_patient_id:** `typing.Optional[str]` — Values should be JSON-encoded, for example filter.patientId="pat_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_service_id:** `typing.Optional[str]` — Values should be JSON-encoded, for example filter.serviceId="svc_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_type:** `typing.Optional[PaymentsListV1FilterType]` — Values should be JSON-encoded, for example filter.type="PATIENT"
    
</dd>
</dl>

<dl>
<dd>

**order_paid_at:** `typing.Optional[PaymentsListV1OrderPaidAt]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/usebridge_api/payments/client.py">create_payment</a>(...) -> PaymentCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payments.create_payment(
    service_id="serviceId",
    paid_at=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    transaction_id="transactionId",
    type="PATIENT",
    amount=1,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `PaymentCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.payments.<a href="src/usebridge_api/payments/client.py">get_payment</a>(...) -> PaymentGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.payments.get_payment(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Policies
<details><summary><code>client.policies.<a href="src/usebridge_api/policies/client.py">get_policy</a>(...) -> PolicyGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.policies.get_policy(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.policies.<a href="src/usebridge_api/policies/client.py">revalidate_policy</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.policies.revalidate_policy(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.policies.<a href="src/usebridge_api/policies/client.py">stream_policy</a>(...) -> typing.Iterator[bytes]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.policies.stream_policy(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Policies V2
<details><summary><code>client.policies.v_2.<a href="src/usebridge_api/policies/v_2/client.py">create_policy</a>(...) -> PolicyCreateV2Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a Policy, returning immediately with status of `PENDING`. Use the Get Policy API, or monitor webhooks, to receive updates.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
from usebridge_api.policies.v_2 import PolicyCreateV2RequestPerson
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.policies.v_2.create_policy(
    person=PolicyCreateV2RequestPerson(
        first_name="firstName",
        last_name="lastName",
        date_of_birth=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    ),
    state="AL",
    payer_id="payerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `PolicyCreateV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ProviderEligibility
<details><summary><code>client.provider_eligibility.<a href="src/usebridge_api/provider_eligibility/client.py">create_provider_eligibility</a>(...) -> ProviderEligibilityCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime
from usebridge_api.provider_eligibility import ProviderEligibilityCreateV1RequestLocation

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.provider_eligibility.create_provider_eligibility(
    date_of_service=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    service_type_id="serviceTypeId",
    location=ProviderEligibilityCreateV1RequestLocation(
        state="AL",
    ),
    payer_id="payerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `ProviderEligibilityCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.provider_eligibility.<a href="src/usebridge_api/provider_eligibility/client.py">get_provider_eligibility</a>(...) -> ProviderEligibilityGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.provider_eligibility.get_provider_eligibility(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Providers
<details><summary><code>client.providers.<a href="src/usebridge_api/providers/client.py">submit_providers</a>(...) -> ProviderPostV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

**Production only:** This endpoint is only available in Production and will not work in Sandbox.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
from usebridge_api.providers import ProviderPostV1RequestProvider

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.providers.submit_providers(
    providers=[
        ProviderPostV1RequestProvider(
            npi="npi",
            email="email",
            caqh_id="caqhId",
            caqh_username="caqhUsername",
            caqh_password="caqhPassword",
        ),
        ProviderPostV1RequestProvider(
            npi="npi",
            email="email",
            caqh_id="caqhId",
            caqh_username="caqhUsername",
            caqh_password="caqhPassword",
        )
    ],
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `ProviderPostV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.providers.<a href="src/usebridge_api/providers/client.py">list_providers</a>(...) -> ProvidersListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.providers.list_providers()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_active:** `typing.Optional[bool]` — Value is a raw boolean, example filter.active=true
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.providers.<a href="src/usebridge_api/providers/client.py">get_provider</a>(...) -> ProviderGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.providers.get_provider(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.providers.<a href="src/usebridge_api/providers/client.py">update_provider</a>(...) -> ProviderUpdateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.providers.update_provider(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ProviderUpdateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Providers Enrollment
<details><summary><code>client.providers.enrollment.<a href="src/usebridge_api/providers/enrollment/client.py">get_provider_enrollment_status</a>(...) -> ProviderEnrollmentStatusGetV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns the high-level enrollment status of a provider

**Production only:** This endpoint is only available in Production and will not work in Sandbox.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.providers.enrollment.get_provider_enrollment_status(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Search
<details><summary><code>client.search.<a href="src/usebridge_api/search/client.py">payer_search</a>(...) -> SearchPayerV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.search.payer_search(
    query="query",
    limit=1,
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `SearchPayerV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ServiceEligibility
<details><summary><code>client.service_eligibility.<a href="src/usebridge_api/service_eligibility/client.py">stream_service_eligibility</a>(...) -> typing.Iterator[bytes]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.service_eligibility.stream_service_eligibility(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.service_eligibility.<a href="src/usebridge_api/service_eligibility/client.py">get_service_eligibility</a>(...) -> ServiceEligibilityGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.service_eligibility.get_service_eligibility(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ServiceEligibility V2
<details><summary><code>client.service_eligibility.v_2.<a href="src/usebridge_api/service_eligibility/v_2/client.py">create_service_eligibility</a>(...) -> ServiceEligibilityCreateV2Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a ServiceEligibility, returns immediately in the `PENDING` status. 
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.service_eligibility.v_2.create_service_eligibility(
    service_type_id="serviceTypeId",
    date_of_service=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    state="AL",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `ServiceEligibilityCreateV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ServiceTypes
<details><summary><code>client.service_types.<a href="src/usebridge_api/service_types/client.py">list_service_types</a>(...) -> ServiceTypesListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.service_types.list_service_types()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.service_types.<a href="src/usebridge_api/service_types/client.py">get_service_type</a>(...) -> ServiceTypeGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.service_types.get_service_type(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Services
<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">stream_service</a>(...) -> typing.Iterator[bytes]</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.stream_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">list_services</a>(...) -> ServicesListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.list_services()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter_service_type_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.serviceTypeId="svt_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_patient_id:** `typing.Optional[str]` — should be JSON-encoded, for example filter.patientId="pat_xxx"
    
</dd>
</dl>

<dl>
<dd>

**filter_status:** `typing.Optional[typing.List[ServicesListV1FilterStatus]]` — should be a JSON-encoded array, for example filter.status=["PENDING", "COMPLETE"]
    
</dd>
</dl>

<dl>
<dd>

**filter_provider_id:** `typing.Optional[typing.List[ServicesListV1FilterProviderId]]` — should be JSON-encoded array, for example filter.providerId=["prv_xxx", "prv_yyy"]
    
</dd>
</dl>

<dl>
<dd>

**order_created_at:** `typing.Optional[ServicesListV1OrderCreatedAt]` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">create_service</a>(...) -> ServiceCreateV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime
from usebridge_api.services import ServiceCreateV1RequestLocation

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.create_service(
    patient_id="patientId",
    date_of_service=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    service_type_id="serviceTypeId",
    location=ServiceCreateV1RequestLocation(
        state="AL",
    ),
    provider_id="providerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `ServiceCreateV1Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">get_service</a>(...) -> ServiceGetV1Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Fetch a Service by `id` or `externalId`
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.get_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">revalidate_service</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.revalidate_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">bill_service</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.bill_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">get_service_note</a>(...) -> ServiceNoteGetV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.get_service_note(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.<a href="src/usebridge_api/services/client.py">delete_service_note</a>(...)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.delete_service_note(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Services Payments
<details><summary><code>client.services.payments.<a href="src/usebridge_api/services/payments/client.py">list_service_payments</a>(...) -> ServicePaymentsListV1Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.payments.list_service_payments(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**page:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**limit:** `typing.Optional[int]` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Services V2
<details><summary><code>client.services.v_2.<a href="src/usebridge_api/services/v_2/client.py">create_service</a>(...) -> ServiceCreateV2Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a new `Service`, creates the `ServiceEligibility` in status `PENDING`
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment
import datetime
from usebridge_api.services.v_2 import ServiceCreateV2RequestLocation

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.v_2.create_service(
    patient_id="patientId",
    date_of_service=datetime.datetime.fromisoformat("2024-01-15T09:30:00+00:00"),
    service_type_id="serviceTypeId",
    location=ServiceCreateV2RequestLocation(
        state="AL",
    ),
    provider_id="providerId",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `ServiceCreateV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.v_2.<a href="src/usebridge_api/services/v_2/client.py">cancel_service</a>(...) -> ServiceCancelV2Response</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.v_2.cancel_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ServiceCancelV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.services.v_2.<a href="src/usebridge_api/services/v_2/client.py">update_service</a>(...) -> ServiceUpdateV2Response</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Updates an existing `Service`
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from usebridge_api import BridgeApiClient
from usebridge_api.environment import BridgeApiClientEnvironment

client = BridgeApiClient(
    api_key="<value>",
    environment=BridgeApiClientEnvironment.PRODUCTION,
)

client.services.v_2.update_service(
    id="id",
)

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `str` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ServiceUpdateV2Request` 
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

